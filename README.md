# GROMACS Protein-Ligand Simulation Guide

![GROMACS](https://img.shields.io/badge/GROMACS-Molecular%20Dynamics-blue)
![License](https://img.shields.io/badge/License-MIT-orange)
![Status](https://img.shields.io/badge/Status-Active-brightgreen)

An interactive, comprehensive guide for running protein-ligand molecular dynamics simulations using GROMACS. This guide provides step-by-step instructions from system preparation to analysis, with a focus on practical implementation and best practices.

## 🌟 Features

- **Complete Workflow**: End-to-end guidance from protein/ligand preparation to simulation analysis
- **Interactive Interface**: Clean, responsive web interface with copy-paste commands
- **Expert Tips**: Professional insights for simulation quality and troubleshooting
- **Case Study**: Complete T4 lysozyme-JZ4 ligand example with expected results
- **Validation Metrics**: Comprehensive criteria for assessing simulation quality
- **Optimized Templates**: Pre-configured MDP files for each simulation phase

## 🚀 Quick Start

### View the Guide
Simply open `GROMACS-Guide.html` in any modern web browser to access the complete interactive guide.

### Prerequisites
- GROMACS (2020+ recommended)
- Python (for ligand parameterization scripts)
- Basic familiarity with command line and molecular dynamics concepts

## 📋 Guide Contents

### 1. **Preparation Phase**
- Protein structure processing with `pdb2gmx`
- Ligand parameterization using ACPYPE/CGenFF
- Complex assembly and topology building
- Force field selection guidance

### 2. **Simulation Phase**
- System solvation and ionization
- Energy minimization protocols
- NVT and NPT equilibration
- 10ns production MD run

### 3. **Analysis Phase**
- Trajectory processing and centering
- RMSD calculations for stability assessment
- Protein-ligand interaction energy analysis
- Binding mode validation

### 4. **Case Study**
Complete workflow example using:
- **System**: T4 Lysozyme L99A/M102Q (PDB: 3HTB)
- **Ligand**: JZ4 (2-propylphenol)
- **Force Field**: CHARMM36
- **Expected Results**: Provided for validation

## 🛠️ Technical Details

### Supported Force Fields
- AMBER (amber99sb-ildn + GAFF2)
- CHARMM (charmm36m + CGenFF) 
- OPLS (oplsaa + ligpargen)

### Simulation Parameters
- **Production Run**: 10ns (configurable)
- **Temperature**: 300K
- **Pressure**: 1 bar
- **Water Model**: TIP3P (default)
- **Ionic Strength**: 150 mM NaCl

### Included MDP Templates
- `minim.mdp` - Energy minimization
- `nvt.mdp` - NVT equilibration  
- `npt.mdp` - NPT equilibration
- `md.mdp` - Production MD
- `ie.mdp` - Interaction energy analysis

## 📊 Validation Metrics

| Metric | Target Value | Interpretation |
|--------|-------------|----------------|
| Protein RMSD | 1.5-3.0 Å | Stable structure |
| Ligand RMSD | < 2.0 Å | Stable binding |
| H-bond Occupancy | >70% | Specific interactions |
| Interaction Energy | -50 to -300 kJ/mol | Strong binding |

## 🎯 Use Cases

- **Drug Discovery**: Protein-ligand binding studies
- **Academic Research**: Molecular dynamics methodology
- **Education**: Teaching MD simulation principles
- **Method Development**: Protocol optimization and validation

## 🔧 Customization

The guide is designed to be adaptable:
- Modify simulation lengths in MDP templates
- Adjust force field combinations
- Extend analysis protocols
- Add new case studies

## 📚 Resources

### External Links
- [GROMACS Manual](https://manual.gromacs.org/)
- [MD Tutorials](http://www.mdtutorials.com/gmx/)
- [CGenFF Server](https://www.charmm-gui.org/)
- [Best Practices Paper](https://pubs.acs.org/doi/10.1021/acs.jcim.5b00654)

### Required Tools
- GROMACS simulation package
- Visualization software (VMD, PyMOL, or Chimera)
- Text editor for file modifications
- Python for auxiliary scripts

## 🤝 Contributing

Contributions are welcome! Please feel free to:
- Report bugs and issues
- Suggest new features
- Add additional case studies
- Improve documentation
- Share your simulation results

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Deon**  
- GitHub: [@Deon-07](https://github.com/Deon-07)
- Project: [GROMACS Simulation Guide](https://github.com/Deon-07/gromacs-guide)

## 🙏 Acknowledgments

- GROMACS development team
- CHARMM force field developers
- MD tutorial communities
- Contributors to open-source molecular modeling tools

---

**Note**: This guide is for educational and research purposes. Always validate your simulation protocols and results against experimental data when available.

---

<div align="center">
  
*Built with ❤️ for the computational biology community*

</div>
