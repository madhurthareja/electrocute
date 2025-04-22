# Electrocute

**Electrocute** is a Python library designed for electronic formulas and signal processing. It provides easy-to-use functions for calculations like Ohm's Law, power, FFT, DFT, and filters, making it ideal for engineers, students, and hobbyists.

---

## Installation

```bash
pip install electrocute
```

## Usage

```python
from electrocute import Electrocute

# Calculate voltage using Ohm's Law
voltage = Electrocute.ohms_law(current=2, resistance=5)
print(f"Voltage: {voltage} V")  # Output: 10 V

import numpy as np
from electrocute import Electrocute

t = np.linspace(0, 1, 1000, endpoint=False)
signal = np.sin(2 * np.pi * 10 * t)
freqs, amps = Electrocute.frequency_spectrum(signal, sampling_rate=1000)
```

## Features

- Electronic formulas (Ohm's Law, power calculations, etc.)
- Signal processing (FFT, DFT, frequency spectrum, filters)
- Extensible and well-documented API

## Contributing

Contributions are welcome! Please submit a pull request or open an issue on GitHub.

### Maintainers:
This library is under development and is actively maintained by Madhur Thareja.

## License

MIT License
