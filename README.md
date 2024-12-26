![Banner](./Screenshots/banner.png)

Welcome to the **Image Recreation Using Genetic Algorithm** project! This application demonstrates the power of genetic algorithms by evolving binary images to closely resemble a target image. Designed as part of an AI course project, it highlights optimization techniques inspired by natural evolution.

---

## 🖋 Table of Contents
1. [Overview](#-overview)
2. [Features](#-features)
3. [Screenshots](#-screenshots)
4. [Installation](#-installation)
5. [Usage](#-usage)
6. [Dependencies](#-dependencies)
7. [Contributors](#-contributors)

---

## 📜 Overview

This project leverages **Genetic Algorithms (GA)** to reconstruct a predefined target image from a random population of binary (black-and-white) images. By employing techniques like selection, crossover, and mutation, the algorithm iteratively evolves toward a solution.

### Key Highlights:
- **Fitness Evaluation**: Matches the generated image to the target based on pixel similarity.
- **Tournament Selection**: Selects parents for producing the next generation.
- **Uniform Crossover**: Combines traits from two parents to create offspring.
- **Mutation**: Introduces randomness to maintain diversity.
- **Replacement Strategy**: Ensures progressive evolution through generations.

---

## ✨ Features

- **Genetic Algorithm Implementation**:
  - Chromosome Representation: Binary images as 2D arrays of 0s and 1s.
  - Fitness Function: Measures the similarity to the target image.
  - Iterative Population Evolution: Progressively improves over generations.

- **Customizable Parameters**:
  - **Population Size**: Number of images per generation.
  - **Mutation Rate**: Likelihood of random pixel flips.
  - **Crossover Rate**: Probability of combining parent traits.

- **Visualization**:
  - Displays generations of images as they evolve toward the target.
    
---

## 🗄 Screenshots

![Main Page](./Screenshots/main-screen.png)

![Recreation of image 1](./Screenshots/recreation-1.png)

![Recreation of image 2](./Screenshots/recreation-2.png)

![Recreation of image 3](./Screenshots/recreation-3.png)

![Recreation of image 4](./Screenshots/recreation-4.png)

---

## 🚀 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/USMAN-FAIZYAB-KHAN/Django-Delights.git
   cd Django-Delights
   ```

2. Create and activate a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install Dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Run the development server:
   ```bash
   python manage.py runserver
   ```

5. Visit `http://127.0.0.1:8000/` to explore the application.

---

## 📖 Usage

1. Set your desired target image:
   - Replace the default target image (`target.png`) in the project directory.

2. Customize algorithm parameters:
   - Modify `population_size`, `mutation_rate`, and `num_generations` in `config.py`.

3. Run the algorithm:
   ```bash
   python main.py
   ```

4. Observe the evolution:
   - Check the `output` directory for the final image and generation progress.

---

## 📦 Dependencies

The following Python libraries are required:

- **Django**: Framework for the web interface.
- **Django Channels**: Real-time WebSocket support for live updates.
- **NumPy**: Efficient array computations.
- **Pillow**: Image handling and processing.

Install all dependencies with:
```bash
pip install -r requirements.txt
```

---

## 🤝 Contributors
- [**Usman Faizyab Khan**](https://github.com/USMAN-FAIZYAB-KHAN)  
- [**Muhammad Zunain**]()  
- **Syed Abdul Basit**

---

Enjoy using this project! Contributions and feedback are welcome. 😊
