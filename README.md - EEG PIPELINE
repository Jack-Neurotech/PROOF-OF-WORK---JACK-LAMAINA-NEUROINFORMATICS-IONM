#1 EEGsignal.py - EEG PIPELINE


# 1. What Is the Project and What Does It Do?

* **Project:** EEG Signal Analysis Pipeline

* **Purpose:** A Python-based neuroinformatics pipeline for loading, processing, analyzing, and reporting EEG recordings.

* **Input:** An EEG recording selected from the computer.

* **Primary goal:** Convert raw EEG recordings into meaningful quantitative measurements that can be used to understand the characteristics of the recorded brain signal.

* **The pipeline performs the following steps:**

  * Loads an EEG recording into Python.
  * Extracts the recorded EEG signal.
  * Identifies information about the recording and its channels.
  * Represents the EEG measurements as numerical data.
  * Calculates basic statistical measurements of the signal.
  * Analyzes the signal in the time domain.
  * Analyzes the signal in the frequency domain.
  * Calculates total spectral power.
  * Identifies the dominant frequency.
  * Identifies peak alpha frequency.
  * Calculates spectral entropy.
  * Calculates spectral edge frequency.
  * Calculates EEG frequency-band power.
  * Calculates relative band power.
  * Calculates band-power ratios.
  * Calculates additional signal measurements such as mean, standard deviation, variance, and RMS.
  * Generates visualizations of the EEG data and analysis results.
  * Organizes the measurements and visualizations into an EEG analysis report.

* **Time-domain analysis:**

  * Examines how the EEG signal changes over time.
  * Measures characteristics such as amplitude and variability.
  * Produces numerical measurements describing the waveform.

* **Frequency-domain analysis:**

  * Examines the frequencies contained within the EEG signal.
  * Measures how much spectral power occurs at different frequencies.
  * Allows the signal to be analyzed according to conventional EEG frequency bands.

* **EEG frequency-band analysis:**

  * Delta
  * Theta
  * Alpha
  * Beta

* **Overall concept:**

  * The project takes an EEG recording as its input.
  * Python converts the recording into data that can be mathematically analyzed.
  * Signal-processing methods extract quantitative features from that data.
  * The resulting features are organized into an interpretable report.

* **In simple terms:**

  * **EEG recording → numerical data → mathematical analysis → signal features → EEG report**

* **What the project demonstrates:**

  * Python programming
  * Scientific computing
  * Numerical data processing
  * Digital signal processing
  * EEG analysis
  * Neuroinformatics
  * Data visualization
  * Reproducible computational analysis
 
    
 
  # 2. Python Principles, General Structure, Packages, and Associated Principles

## A. Python Principles and the General Structure

The EEG pipeline is built from fundamental Python programming concepts. These concepts provide the structure that allows the scientific packages and EEG-processing operations to work together.

### Variables

* Variables store information so the program can use it later.
* An EEG signal, sampling rate, filename, frequency, or calculated measurement can all be stored in variables.

```python
sampling_rate = 500
```

In this example:

* `sampling_rate` is the variable.
* `500` is the value stored inside the variable.

---

### Data Types

Python can store different kinds of information.

Common types used in the pipeline include:

* **Numbers** — measurements such as frequency or amplitude.
* **Strings** — filenames, channel names, and labels.
* **Lists** — collections of values.
* **Arrays** — large numerical datasets.
* **Objects** — organized structures containing data and functionality.

Example:

```python
channel_name = "Fp1"
sampling_rate = 500
```

The first variable contains text, while the second contains a number.

---

### Lists and Collections

A list allows multiple pieces of information to be stored together.

```python
channels = ["Fp1", "Fp2", "F3", "F4"]
```

The program can then work through the channels individually.

---

### Indexing

Indexing allows Python to access a specific item inside a collection.

```python
channels[0]
```

This accesses the first item.

Indexing is important when working with individual EEG samples or channels.

---

### Slicing

Slicing allows the program to extract a section of a collection.

```python
signal[0:1000]
```

This can be used to select a section of EEG data instead of processing the entire recording at once.

---

### Functions

Functions organize operations into reusable pieces of code.

```python
def analyze_signal(signal):
    ...
```

A function can:

1. Receive input.
2. Process the input.
3. Return a result.

The general structure is:

**Input → Processing → Output**

Functions make the EEG pipeline modular because individual analysis operations can be reused.

---

### Loops

Loops allow Python to repeat an operation.

```python
for channel in channels:
    analyze(channel)
```

Instead of writing the same analysis four times, the program can repeat the operation for every channel.

This becomes particularly important when an EEG recording contains many channels.

---

### Conditional Statements

Conditional statements allow the program to make decisions.

```python
if data_exists:
    analyze(data)
```

Conditions allow the pipeline to respond differently depending on what happens during execution.

They can be used to:

* Check whether data exists.
* Check whether a file was successfully loaded.
* Determine whether a channel is available.
* Decide whether a graph should be displayed.
* Handle different analysis conditions.

---

### Imports

Imports allow one Python file to access functionality created elsewhere.

```python
import numpy as np
import mne
```

The pipeline uses imports to connect Python's basic programming structure to specialized scientific libraries.

---

### Objects

Objects allow complex information to be organized into a single structure.

For EEG analysis, an object can represent an entire recording and contain information such as:

* Signal data
* Channels
* Sampling rate
* Metadata
* Recording information

Objects allow the program to work with the recording as one organized entity.

---

### Methods

Methods are functions associated with an object.

For example:

```python
object.method()
```

The method performs an operation using the information contained in that object.

This is especially important when working with MNE EEG recordings.

---

### Errors and Exceptions

Python can encounter problems while running the pipeline.

For example:

* A file may not exist.
* An EEG recording may be missing required information.
* A channel may not be available.
* A package may not be installed.

Python provides exceptions so the program can identify and respond to these problems rather than silently producing incorrect results.

---

## General Structure of the EEG Pipeline

The fundamental structure of the EEG pipeline is:

**1. Input**

* Locate an EEG recording.
* Select the file.
* Load the recording.

**2. Data Representation**

* Represent the EEG recording as an object.
* Extract the numerical signal data.
* Identify channels and recording parameters.

**3. Numerical Processing**

* Store the signal as numerical data.
* Calculate basic signal statistics.
* Examine the signal in the time domain.

**4. Signal Processing**

* Transform the signal into the frequency domain.
* Calculate spectral power.
* Identify frequency characteristics.
* Calculate EEG frequency-band measurements.

**5. Feature Extraction**

The pipeline can calculate meaningful measurements such as:

* Mean
* Standard deviation
* Variance
* RMS
* Total spectral power
* Dominant frequency
* Peak alpha frequency
* Spectral entropy
* Spectral edge
* Band-power ratios

**6. Visualization**

* Plot the EEG waveform.
* Plot frequency information.
* Display calculated measurements.

**7. Report**

* Combine the calculated information into a structured EEG analysis report.

The overall computational pattern is therefore:

**EEG File → Load → Extract → Process → Analyze → Calculate Features → Visualize → Report**

---

# B. Packages and the Python Principles Associated With Them

## NumPy

**Purpose:**

* Numerical computing.
* EEG signals contain large numbers of numerical samples.
* NumPy provides arrays for efficiently storing and processing those samples.

### Python principles associated with NumPy

* Variables
* Arrays
* Indexing
* Slicing
* Functions
* Mathematical operations
* Iteration

Example:

```python
signal = np.array([...])
```

The EEG signal becomes a numerical array that Python can analyze.

NumPy can then perform calculations such as:

```python
np.mean(signal)
```

```python
np.std(signal)
```

```python
np.var(signal)
```

These operations form the numerical foundation of the EEG analysis.

---

## SciPy

**Purpose:**

* Scientific computing.
* Signal processing.
* Frequency-domain analysis.

SciPy provides specialized mathematical and signal-processing functions that would otherwise have to be implemented manually.

### Python principles associated with SciPy

* Functions
* Variables
* Arrays
* Mathematical operations
* Function inputs and outputs
* Iteration

For example, a signal-processing function can receive an EEG array and return frequency-related information.

The general structure is:

**EEG Array → SciPy Function → Processed Data**

In this project, SciPy is used for operations such as:

* Spectral analysis
* Periodograms
* Frequency analysis
* Signal processing
* Power calculations
* Frequency-band analysis

---

## MNE

**Purpose:**

* Working with EEG and other electrophysiological recordings.
* Loading and organizing neurophysiological data.
* Providing access to recording information.

MNE is the package that connects the general Python program to the structure of an actual EEG recording.

### Python principles associated with MNE

* Imports
* Objects
* Methods
* Attributes
* Variables
* Functions

An EEG recording can be represented as an MNE object.

That object can contain information about:

* EEG signals
* Channels
* Sampling frequency
* Recording metadata
* Timing information

The general relationship is:

**EEG File → MNE Object → EEG Data**

MNE therefore handles the neurophysiological data structure, while NumPy and SciPy perform much of the numerical analysis.

---

## Matplotlib

**Purpose:**

* Data visualization.
* Converts numerical analysis into visual graphs.

### Python principles associated with Matplotlib

* Imports
* Functions
* Objects
* Methods
* Variables

For example:

```python
plt.plot(times, signal)
```

The program provides Matplotlib with:

* Time values.
* EEG signal values.

Matplotlib converts those values into a waveform.

It can therefore visualize:

* EEG voltage over time.
* Frequency spectra.
* Spectral power.
* Other calculated EEG features.

---

## pathlib

**Purpose:**

* Managing files and directories.
* Finding EEG recordings on the computer.
* Creating structured file paths.

### Python principles associated with pathlib

* Objects
* Variables
* Methods
* Operators

Example:

```python
from pathlib import Path

downloads = Path.home() / "Downloads"
```

Python represents the file location as a `Path` object.

This allows the program to work with files without manually constructing operating-system-specific paths.

---

## subprocess

**Purpose:**

* Allows Python to communicate with operating-system processes.
* In the EEG pipeline, this supports interaction with macOS functionality used for file selection.

### Python principles associated with subprocess

* Functions
* Variables
* External processes
* Return values
* Error handling

The general concept is:

**Python → Operating System → Result → Python**

This allows the Python program to interact with functionality outside of Python itself.

---

## How the Packages Work Together

The packages are not independent pieces of the project. Each performs a different part of the computational process.

**MNE**

→ Loads and organizes the EEG recording.

**NumPy**

→ Represents and numerically processes the EEG samples.

**SciPy**

→ Performs scientific and signal-processing analysis.

**Matplotlib**

→ Turns the resulting data into visualizations.

**pathlib**

→ Handles file locations.

**subprocess**

→ Connects Python with operating-system functionality.

The Python programming principles provide the structure connecting all of them:

**Variables → Functions → Objects → Methods → Conditions → Loops → Data Processing → Output**

Together, these principles and packages form the computational foundation of the EEG pipeline.

3. Statistics

   
Mean — the average value of the EEG signal.
Standard Deviation — measures how much the EEG values vary around the mean.
Variance — measures the overall spread or variability of the EEG values.
Minimum — the lowest value recorded in the EEG signal.
Maximum — the highest value recorded in the EEG signal.
RMS (Root Mean Square) — measures the overall magnitude of the EEG signal.
Total Spectral Power — the total amount of signal power across the analyzed frequency range.
Dominant Frequency — the frequency containing the greatest amount of spectral power.
Peak Alpha Frequency — the frequency within the alpha range with the greatest spectral power.
Spectral Entropy — measures how evenly the signal's power is distributed across frequencies.
Spectral Edge Frequency — the frequency below which a specified percentage of the total spectral power is contained.
Band Power — the amount of signal power contained within a specific frequency band.
Relative Band Power — the proportion of total spectral power contained within a specific frequency band.
Band-Power Ratio — compares the power of one frequency band with another.
Channel ID — identifies the EEG channel from which the signal was recorded.
Channel Location — identifies the electrode's anatomical or scalp position, such as Fp1, Fp2, or F3.
Sampling Rate — the number of EEG samples recorded per second.
Signal Duration — the length of time represented by the EEG recording or analyzed segment.


