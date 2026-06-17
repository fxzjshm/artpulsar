# Artificial Pulsar signal generator

Generate and send artificial pulsar signal with USRP.

Related paper: An Artificial Pulsar-signal Generator for Pulsar Search, <https://iopscience.iop.org/article/10.1088/1674-4527/ae3f08>, DOI: 10.1088/1674-4527/ae3f08

Build:

```bash
make
# or
make -f Makefile.cpu
```

Example usage:

```bash
./tx_pulsar --cohmod --gain 70 --dm 50 --pms 134 --rate 16000000 --freq 100000000
```

refer to `--help` for usage.
