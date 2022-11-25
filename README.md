# Ransomwhere

A Proof of Concept ransomware sample that encrypts your files to test out your ransomware detection & prevention strategies.</br>
I am not responsible for any damage caused by this software.

If no arguments are provided, `ransomwhere`will automatically execute the `encrypt` mode without deleting the original files.

## Building

```shell
# with make and Go installed
% make build
```

## Usage

```shell
# straight from source
% make FLAGS="-log=warn -delete=false -mode=encrypt"

# from the binary
% ./app -log=warn -delete=false -mode=encrypt

# encrypt AND delete files like a real ransomware (DANGEROUS)
% ./app -delete=true
```