![Banner](./Screenshots/banner.png)

Welcome to the **Image Recreation Using Genetic Algorithm** project! This application demonstrates the power of genetic algorithms by evolving binary images to closely resemble a target image. Featuring a Django-powered web interface with real-time updates via **Django Channels**, users can interact with the algorithm in a seamless and dynamic environment. It also highlights optimization techniques inspired by natural evolution.

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

With the Django web interface, users can upload target images and monitor real-time updates of the evolution process via **WebSockets**, powered by **Django Channels**.  

### Key Highlights:
- **Real-Time Updates**: View generation progress instantly via WebSockets.
- **Fitness Evaluation**: Matches the generated image to the target based on pixel similarity.
- **Tournament Selection**: Selects parents for producing the next generation.
- **Uniform Crossover**: Combines traits from two parents to create offspring.
- **Mutation**: Introduces randomness to maintain diversity.
- **Replacement Strategy**: Ensures progressive evolution through generations.
  
---

## ✨ Features

- **Interactive Web Interface**:
  - Upload target images or select any of the existing images.
  - View real-time evolution updates and the final results.

- **Genetic Algorithm Implementation**:
  - Chromosome Representation: Binary images as 2D arrays of 0s and 1s.
  - Fitness Function: Measures the similarity to the target image.
  - Iterative Population Evolution: Progressively improves over generations.

- **Real-Time Functionality**:
  - Built with Django Channels for WebSocket-based updates.
  - Watch the evolution process live without refreshing the page.
    
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

1. Upload or select an image from the web interface.  
2. The genetic algorithm starts automatically after the image is selected or uploaded.  
3. View live updates of the recreation process on the web interface.  
4. The final recreated image is displayed upon completion.  

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

### 🧑‍💻 Technical Details: Genetic Algorithm Flow  

1. **Initialization**: Create a population of random binary images, each pixel representing a gene (0 or 1).  
2. **Fitness Evaluation**: Measure similarity to the target image by counting matching pixels.  
3. **Selection**: Use tournament selection to choose parent images based on fitness.  
4. **Crossover**: Combine parents using uniform crossover, mixing traits via a random mask.  
5. **Mutation**: Flip a small percentage of pixels to introduce diversity.  
6. **Replacement**: Replace the old population with offspring to progress toward the target image.  
7. **Convergence**: Repeat for multiple generations until the population closely matches the target.  

---

## 🤝 Contributors
- [**Usman Faizyab Khan**](https://github.com/USMAN-FAIZYAB-KHAN)  
- [**Muhammad Zunain**]()  
- **Syed Abdul Basit**

---

Enjoy using this project! Contributions and feedback are welcome. 😊
