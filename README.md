# My Personal CV Written in LaTeX

This repository contains my CV written in LaTeX with a modular and clean structure.

## 📁 Structure

```
.
├── main.tex                 # Main file to compile
├── preamble.tex             # Configuration and packages
└── sections/                # Sections folder for organization and modularity
    ├── header.tex
    ├── skills.tex
    ├── experience.tex
    ├── projects.tex
    └── education.tex
```

## 🛠️ Compile

The preamble uses `fontspec`, so build with XeTeX (or LuaTeX), not `pdflatex`. From `src/`, either run Tectonic through Nix (no TeX install needed):

```bash
nix --extra-experimental-features 'nix-command flakes' run nixpkgs#tectonic -- -o output main.tex
```

or, with TeX Live installed:

```bash
xelatex -output-directory=output main.tex
```

## 🔗 Links

- Website: [https://msdqn.dev](https://msdqn.dev)
- GitHub: [https://github.com/maulanasdqn](https://github.com/maulanasdqn)
- Email: [maulanasdqn@gmail.com](mailto:maulanasdqn@gmail.com)

## 📄 License

Feel free to fork and adapt for personal use.
