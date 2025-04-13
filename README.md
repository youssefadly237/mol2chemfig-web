# Mol2chemfig Web

**Mol2chemfig Web** is a web interface for the **Mol2chemfig** program, which is maintained by [Prof. M. Palmer](https://www.soas.ac.uk/about/michael-palmer). The purpose of the project is to offer a user-friendly platform for generating and modifying chemical structures in the **chemfig** format for LaTeX documents. The web application includes the following features:

## Features

### **Integrated Database Search**

Search for a compound by name and retrieve its corresponding SMILES string.

### **Integrated ChemDoodle Sketcher**

If a compound is not found in the database, the user can draw its structure using the [ChemDoodle sketcher](http://web.chemdoodle.com/tutorial/2d-structure-canvases/sketcher-canvas). The resulting structure is then converted into MOL format.

### **Embedded PDF Viewer**

Once a SMILES or MOL format is converted into chemfig, the generated structure is displayed in the embedded PDF viewer.

### **"Select - Apply" Functionality**

The user can modify the structure by selecting various options, which are then applied. The updated PDF reflects the changes. Currently, ten options are available, and more can be added upon request.

### **Live Updates on Chemfig Code Modifications**

Users can modify the chemfig code directly, such as changing the bond angle or functional groups. Every modification is immediately reflected in the PDF viewer.

## Installation

To run Mol2chemfig Web locally, the following packages need to be installed:

- [Flask](https://flask.palletsprojects.com/en/stable/) - `pip install Flask`
- [Pubchempy](pubchempy.readthedocs.io) - `pip install pubchempy`
- Indigo - `pip install epam.indigo`
- Pdflatex

Additionally, you'll need to update the path to the **mol2chemfig.sty** file (defined as `m2pkg_path` in `mol2chemfig/pdfgen.py`) for the PDF generation process.

## Acknowledgments

I would like to acknowledge the authors of the following programs/libraries used in developing this web interface:

- **Chemfig**  
- **Mol2chemfig**  
- **ChemDoodle Web Components**  
- **PubchemPy**  
- **Indigo**

## License

Mol2chemfig Web (web interface only) is licensed under version 3 of the [GNU GENERAL PUBLIC LICENSE](https://www.gnu.org/licenses/gpl-3.0.html).

## Comments, Suggestions, and Bug Reports

Your feedback, suggestions, bug reports, and constructive criticism are highly appreciated. Please send them to:  
**Email**: [Youssef Adly](youssefadly237@gmail.com)

## Attention

This is an old repository that I have cloned to improve; this markdown is not yet updated.

## Plan

- Update the web interface to support the latest versions of dependencies.
- Refactor the codebase for improved maintainability.
- Enhance the user interface for a better user experience.
- Add naming to what you have drawn.
