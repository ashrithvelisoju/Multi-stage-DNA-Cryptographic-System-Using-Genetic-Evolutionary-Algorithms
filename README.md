# DNA Encryption Studio 🧬

A sophisticated web application for encrypting and decrypting DNA sequences using genetic pattern recognition and binary transformation algorithms. Built with Streamlit, this tool provides an intuitive interface for bioinformatics researchers, cryptography enthusiasts, and students to explore DNA-based encryption methodologies.

## Overview

The DNA Encryption Studio implements a novel approach to cryptographic systems by leveraging genetic evolutionary algorithms and DNA sequence patterns. The application segments DNA sequences, classifies them based on genetic patterns (Mutated, Crossover, Reshape), and applies binary encoding with functional mapping to create encrypted outputs.

## Modules

- **Pre-processing**
- **Encryption**
- **Reshaping**
- **Crossover**
- **Mutation**

## Abstract

This technique takes binaries of any type of digital data and converts them to DNA sequencing format, then applies reshaping, encryption, crossover, and mutation operations. The main stages of D-GET are repeated three times or more to enhance security. The encrypted data is transmitted in text/image format files.

On the receiver side, D-GET is used to decrypt the received data and reshape it back to its original format. This technique employs multiple key sequences to increase the degree of diffusion and confusion, making the resulting cipher data extremely difficult to decipher and realizing a perfect secrecy system.

Experimental results demonstrate that the proposed technique provides:
- Multilayer protection against different types of attacks
- Higher level of security through multi-stage processing
- Genetic operations for enhanced cryptographic strength
- Symmetric key cryptography implementation
- Random key generation capabilities

## Processing Stages

### 1. Pre-processing Stage

- Reads secret data and prepares it based on its type
- For text files: converts to ASCII values
- Groups data into 8-bit binary format
- Maps every two adjacent bits to four DNA bases:
  - **A** (Adenine)
  - **C** (Cytosine)  
  - **G** (Guanine)
  - **T** (Thymine)

### 2. Encryption Stage

- Converts binary data to DNA sequencing
- Encrypts using a variable-length key (DNA sequence or binary string)
- If data and key are DNA sequences:
  - Converts to binary form
  - Performs XOR operation on corresponding elements
  - Converts back to DNA sequence

### 3. Reshaping Stage

- Implements basic genetic algorithm with three operators:
  - Reproduction
  - Crossover
  - Mutation
- Determines chromosome number and length (constant or variable per round)
- Aligns DNA sequence into rows to construct parent chromosomes with predefined length

### 4. Crossover Stage

- Selects parents in the mating pool
- Implements two types of crossover (used sequentially in technique rounds):
  1. **Single-point crossover**: 
     - Selects crossover point between first and last bits
     - Creates two offspring by exchanging heads of parent1 and parent2
     - Offspring contain DNA code portions from both parents

### 5. Mutation Stage

- Applies alteration to string elements
- Implements two mutation types:
  1. **Single-point mutation**:
     - Converts data to binary vector
     - Defines two mutation points
     - Complements bits in between (1→0, 0→1)
  2. **DNA base mutation**:
     - Converts four bits to two DNA bases (e.g., 1010 → CG)
     - Reshapes to DNA bases vector
     - Defines two points and alters DNA bases (e.g., C → G)

## Input/Output

- **Input**: Normal text data
- **Output**: Encrypted and decrypted data using DNA-Genetic Encryption Technique

## Features

- ✅ Multilayer security architecture
- ✅ DNA sequencing-based encryption
- ✅ Genetic algorithm operations
- ✅ Symmetric key cryptography
- ✅ Random key generation
- ✅ Multiple rounds of processing
- ✅ Protection against various attack vectors
- ✅ Perfect secrecy implementation

## Security Benefits

- High degree of diffusion and confusion
- Resistance to cryptanalytic attacks
- Multiple security layers through genetic operations
- Variable key lengths for enhanced security
- DNA-based encoding adds biological complexity layer
  

## Key Features

### 🔬 Core Functionality
- **DNA Sequence Encryption**: Transform DNA sequences into encrypted binary outputs using genetic pattern recognition
- **Decryption with Validation**: Decrypt encrypted sequences and validate against original inputs
- **Custom Key Support**: Apply user-defined encryption keys for enhanced security
- **Real-time Analysis**: Live nucleotide distribution analysis and sequence metrics

### 📊 Visualization & Analytics
- **Interactive Dashboards**: Comprehensive analytics with nucleotide distribution charts
- **Segment Classification Visualization**: Visual representation of genetic pattern classifications
- **Progress Tracking**: Real-time encryption/decryption progress indicators
- **Comparative Analysis**: Side-by-side comparison of original vs. decrypted sequences

### 🗄️ Dataset Integration
- **Hugging Face Integration**: Direct access to genomic datasets from Hugging Face Hub
- **Featured Datasets**: Pre-configured access to canonical human gene sequences
- **Dataset Browser**: Interactive exploration of sequence properties and metadata
- **Sample Generation**: Random sequence generation with configurable GC content bias

### 🎨 User Experience
- **Dual Theme Support**: Light and dark mode interfaces
- **Responsive Design**: Mobile-friendly layout with adaptive components
- **Export Capabilities**: Download results in JSON and FASTA formats
- **Session Management**: Save and restore encryption data across sessions

## Prerequisites

### System Requirements
- Python 3.7 or higher
- 4GB RAM minimum (8GB recommended for large datasets)
- Internet connection for dataset access

### Required Python Packages
```bash
streamlit>=1.28.0
pandas>=1.5.0
numpy>=1.21.0
matplotlib>=3.5.0
plotly>=5.0.0
altair>=4.0.0
datasets>=2.0.0
requests>=2.28.0
Pillow>=9.0.0
