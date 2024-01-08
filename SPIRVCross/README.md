## Details

- Main repo: [SPIRV-Cross](https://github.com/KhronosGroup/SPIRV-Cross)
- License [Apache v2.0](https://github.com/KhronosGroup/SPIRV-Cross/blob/main/LICENSE)

On Windows, Mac or Linux:

```bash
git clone https://github.com/KhronosGroup/SPIRV-Cross
cd SPIRV-Cross
mkdir Release
cd Release
cmake ..
cmake --build . --config Release
```

```
# For: commit f349c91274b91c1a7c173f2df70ec53080076191 (HEAD -> main, origin/main, origin/HEAD)
certutil -hashfile .\spirv-cross.exe SHA512
SHA512 hash of .\spirv-cross.exe:
431f83bca633321036a766834bd88df462cf4b4ab4c03c262bf6391b7c56e14136f6a87742fe2dda769cdcc3efe16c0b8beda1933a9bf88ba2aeb35f9169f89d
CertUtil: -hashfile command completed successfully.
```

TODO: Need a GitHub Action to sign the binary / produce reproducible build. 
For now, one can reproduce my binary by checking out the commit above and building from scratch.