# Flint-GMP-MPFR-Install-Script-Linux
Bash installation script to get FLINT, GMP and MPFR running for some indecent computations lol

## Getting Started

### Cloud/Runpod Installation

First install m4 
```
sudo apt-get update
sudo apt-get install -y m4
```

Then follow the local installation section below.

### Local Installation
1. Check Download.sh and ensure you're working with your desired library versions.
2. Clone the repo.
```
git clone https://github.com/MurageKibicho/Flint-GMP-MPFR-Install-Script-Linux.git
```
3.  cd into the folder.
```
cd Flint-GMP-MPFR-Install-Script-Linux
```

4. Make sure the library versions in `Download.sh` align with your goals.

5. Make Download.sh executable, run Download.sh
```
chmod +x Download.sh

./Download.sh
```

6. Run sample program
I installed Flint in home. Modify this command to match your build

```
clear && gccmain.c -o m.o   -I/home/Flint-GMP-MPFR-Install-Script-Linux/build/local/include   -L/home/Flint-GMP-MPFR-Install-Script-Linux/build/local/lib   -lflint -lmpfr -lgmp -lm   -Wl,-rpath,/home/Flint-GMP-MPFR-Install-Script-Linux/build/local/lib   && ./m.o
```

### Google Colab installation
You can use the provided Jupyter Notebook to get it running on Colab at this [link](https://colab.research.google.com/drive/1mvH_wK0glX4veMPj8s6Aplz8IhqbC811#scrollTo=ZDXZWbx2y1HX)
