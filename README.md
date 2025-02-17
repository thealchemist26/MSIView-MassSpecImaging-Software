Mass Spectrometry Imaging (MSI) Visualizer is a Python package designed to visualize and analyze mass spectrometry imaging data stored in imzML format. The tool enables researchers to explore molecular distributions across tissue samples through an interactive visualization interface.

Let's look at how the visualization workflow operates:
![image](https://github.com/user-attachments/assets/0411ba30-46c2-4ea4-8719-043a6fddf091)


The diagram above illustrates the key components of the MSI Visualizer:

Blue boxes represent input and initialization stages
Green boxes show data processing steps
Orange boxes indicate visualization outputs
Key terms:

m/z: Mass-to-charge ratio, used to identify different molecules
Intensity map: Spatial distribution of molecule concentrations
Colorbar: Scale showing intensity values mapped to colors
Installation

pip install pyimzml numpy matplotlib
Usage Example

from mass_spec_imaging_viewer.MSIVisualizer import MSIVisualizer

# Initialize viewer with imzML file
visualizer = MSIVisualizer("path/to/your/file.imzml")

# Display initial view
visualizer.update_plot()

# Explore different m/z values
visualizer.set_mz(500)  # View distribution of m/z 500
visualizer.set_mz(283.26)  # View distribution of m/z 283.26
Features
Interactive visualization of mass spectrometry imaging data
Real-time m/z value adjustment
Automatic intensity normalization
Efficient batch processing for large datasets
Customizable visualization parameters

Requirements
Python 3.x
pyimzml
numpy
matplotlib
