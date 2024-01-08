## DirectX Shader Compiler

- Main repo [here](https://github.com/microsoft/DirectXShaderCompiler/)
- Binaries from [here](https://github.com/microsoft/DirectXShaderCompiler/releases/tag/v1.7.2308)
- License [University of Illinois/NCSA](https://github.com/microsoft/DirectXShaderCompiler/blob/main/LICENSE.TXT)
  - More info [here](https://en.wikipedia.org/wiki/University_of_Illinois/NCSA_Open_Source_License) - roughly that of BSD/MIT license.

Verify that the SHA512 matches that of the release above:

```bat
# Windows
cd DXShaderCompiler\Windows\x64
certutil -hashfile .\dxc.exe SHA512
SHA512 hash of .\dxc.exe:
5fbd706bf493ef66b76bd76df2691c9145d9fa8e27836e2e7936f175fbcaf64a9a5031b01d04ff6e5880b8b6d999cbc1882d4af2d865aa01a5c60efca8e74344
CertUtil: -hashfile command completed successfully.

certutil -hashfile .\dxcompiler.dll SHA512
SHA512 hash of .\dxcompiler.dll:
a19675916adffeecc027cb0aaa913adb17caf67f2a7f6e60e97c3733ae87de2ad219e64f39a0a3f60b0c749e4331a8f65595a404e7a65117ba4363d68c072401
CertUtil: -hashfile command completed successfully.

certutil -hashfile .\dxil.dll SHA512
SHA512 hash of .\dxil.dll:
3d8c51ae549449b77eeca0139ef07448a3139bcde1b0c55dc4e9f13e39e1a78f51d357b7fff2b3c34b2360abda2b078c32369455a5ebfda16bdee71870a7b758
CertUtil: -hashfile command completed successfully.

```

```sh
# Linux or Mac
cd DXShaderCompiler/Linux
 shasum -a 512 dxc
1fa2c3c0d8e7e1bf5405a6456bebaf2b921e87bcfa17f377d4133b3800b53503083f25c7c28f7034d6222105236535159f4bb17946c168035ce85201c74b6dbf  dxc
```