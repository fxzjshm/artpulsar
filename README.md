# Artificial Pulsar Signal Generator

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

This gives an artificial pulsar signal at center frequency 100 MHz with 16 MHz bandwidth,
134 ms period, DM = 50, and can be coherently de-dispersed.

Please refer to `--help` for usage.

It usually takes several seconds to one minute to calculate required signals and then operate normally.
If any "U" character is shown after about 1 minute, possibly there exists packet loss 
and the output signal may no longer maintain integrity. In this case, try lower "rate" parameter.
