# DNA Encryption Studio 🧬

A sophisticated web application for encrypting and decrypting DNA sequences using genetic pattern recognition and binary transformation algorithms. Built with Streamlit, this tool provides an intuitive interface for bioinformatics researchers, cryptography enthusiasts, and students to explore DNA-based encryption methodologies.

## Overview

The DNA Encryption Studio implements a novel approach to cryptographic systems by leveraging genetic evolutionary algorithms and DNA sequence patterns. The application segments DNA sequences, classifies them based on genetic patterns (Mutated, Crossover, Reshape), and applies binary encoding with functional mapping to create encrypted outputs.

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
