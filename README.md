# GNU Radio Simulated Jammer

GNU Radio flowgraph that receives a real FM station with an RTL-SDR and adds a jamming carrier digitally, showing how interference affects the spectrum and the demodulated audio.

> **Nothing is transmitted.** The RTL-SDR is receive-only, and the interference only exists as samples added in software.

The full explanation is in the article: [Blog](https://getuliovictor.github.io/)

## Requirements

- GNU Radio 3.10
- SoapySDR with the RTL-SDR module (`soapyrtlsdr` on Arch, `soapysdr-module-rtlsdr` on Debian/Ubuntu)
- RTL-SDR dongle

## Usage

Open `simulated_jammer.grc` in GNU Radio Companion, or run the generated script:

```bash
python3 simulated_jammer.py
```

Set `freq` to a local FM station and increase `JAMMING_Power`.
