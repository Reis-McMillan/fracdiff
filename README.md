# fracdiff-modern

**Super-fast fractional differentiation for NumPy, PyTorch, and Scikit-Learn.**

`fracdiff-modern` is a maintained, modernized fork of the original `fracdiff` library. 
It features:
* **Python 3.10 - 3.13+ Support.**
* **Modern Build System**: Fully compatible with `pyproject.toml` and `setuptools >= 77`.

## Installation

Install the base package with NumPy and SciPy:
```sh
pip install fracdiff-modern
```

To use `fracdiff-modern` with Scikit-Learn or PyTorch functionality, install the extras:
```sh
pip install fracdiff-modern[sklearn,torch]
```

## Contributing

Any contributions are more than welcome.

See [Issue](https://github.com/Reis-McMillan/fracdiff/issues) for proposed features.
Please take a look at [CONTRIBUTING.md](.github/CONTRIBUTING.md) before creating a pull request.

## Acknowledgements

This package is a modernization of the original `fracdiff` library by **Shota Imaki**. The core algorithms and logic are based on his work in fractional calculus for financial time series.

## License

BSD-3-Clause License. See [LICENSE](LICENSE) for the full text.

## References

- [Marcos Lopez de Prado, "Advances in Financial Machine Learning", Wiley, (2018).][prado]

[prado]: https://www.wiley.com/en-us/Advances+in+Financial+Machine+Learning-p-9781119482086
