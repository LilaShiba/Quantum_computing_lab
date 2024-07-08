<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" type="text/css" href="styles.css">
</head>
<body>

<h1><a href="https://youtu.be/7UuUOXfiz9Q?si=eZvPbhvttn-waPDz">What is Light?</a></h1>

<p>By the end of this lab, you will be able to explain the quantum properties of light using either Dirac Notation, experimentation results, or graphs produced by your own program.</p>

<h2>🪄 Photons: The Tricksters of Light 🪄</h2>

<p>Photons are the tiny particles that make up light, but they don't always play by the rules we expect! 🌟🔍 Unlike arrows that fly straight and true, photons can be in multiple places at once, interfere with themselves, and even communicate faster than the speed of light! 🚀✨ Let's explore some of these magical behaviors through the lens of quantum computing.</p>

<h2>🔍 Understanding Vectors 🔍</h2>

<p>Before we dive deeper into our quantum adventure, let's take a moment to understand vectors, which are fundamental to quantum computing.</p>

<h3>What is a Vector?</h3>
<p>A vector is a quantity that has both magnitude (size) and direction. Think of it as an arrow: the length of the arrow represents the magnitude, and the way it points represents the direction.</p>

<img src="https://github.com/LilaShiba/Quantum_Collapse_Neuron/blob/main/imgs/qubit_ex.png" alt="Layer 3">

<h3>How Do We Use Vectors in Quantum Computing?</h3>
<p>In quantum computing, vectors help us represent quantum states. For example, a single qubit (the basic unit of quantum information) can be represented as a vector in a two-dimensional space. This vector tells us the probabilities of the qubit being in different states.</p>

<h3>Vectors in Bra-Ket Notation</h3>
<details>
    <summary>Braket Notation in Quantum Mechanics 🧙‍♀️🔮</summary>
    <br>
    <p>In quantum mechanics, <a href='https://en.wikipedia.org/wiki/Bra%E2%80%93ket_notation'>bra-ket notation</a> is essential for representing quantum states and operations.</p>
    <ul>
        <li><strong>Ket |α⟩</strong>: Represents a quantum state vector. Example: |α⟩ could denote the state of a particle. 🌌</li>
        <li><strong>Bra ⟨β|</strong>: The conjugate transpose of a ket, helps for quick computations over all state space. 🔄</li>
        <li><strong>Inner Product ⟨β|α⟩</strong>: Represents the probability amplitude between states |β⟩ and |α⟩. ✨</li>
        <li><strong>Outer Product |α⟩⟨β|</strong>: An operator that projects onto the state |α⟩. 🌀</li>
    </ul>
    <p>Example in a qubit system:</p>
    <ul>
        <li><strong>Kets</strong>: |0⟩, |1⟩</li>
        <li><strong>Bras</strong>: ⟨0|, ⟨1|</li>
        <li><strong>Inner Product</strong>: ⟨0|1⟩ = 0 (shows orthogonality) 🌠</li>
        <li><strong>Outer Product</strong>: |0⟩⟨0| (a projection operator) 🌙</li>
    </ul>
</details>

<h2>🧪 Experiment: Polarized Light and Quantum States 🧪</h2>

<p>Now, let's tie this understanding of vectors into our experiment. We'll be passing light through three layers of polarized film to demonstrate quantum properties.</p>

<h3>What Are Polarized Films?</h3>
<p>Polarized films are materials that only allow light waves vibrating in a certain direction to pass through. When light passes through these films, its direction (or polarization state) changes, much like how vectors can change direction.</p>

<h4>Our Experiment Setup</h4>
<details>
<summary><strong>Start Your Quantum Adventure Here!</strong></summary>
<br>
  
<ol>
  <li><strong>Hardware:</strong> Create a program to measure light in lux using Python & the Raspberry Pi.</li>

  <img src="https://cdn-learn.adafruit.com/assets/assets/000/109/050/medium640/adafruit_products_VEML7700_RasPi_original.jpg?1645044837" alt="Hardware setup">

  <li><strong>Layer 1:</strong> The first layer of polarized film will align the photons in a specific direction.</li>

  <img src="https://alienryderflex.com/polarizer/01.gif" alt="Layer 1">

  <li><strong>Layer 2:</strong> The second layer, oriented at a different angle, will alter the photons' directions further.</li>

  <img src="https://alienryderflex.com/polarizer/02.gif" alt="Layer 2">
  
  <li><strong>Layer 3:</strong> The third layer will demonstrate how the final direction of the photons is influenced by the previous two layers.</li>

  <img src="https://alienryderflex.com/polarizer/03.gif" alt="Layer 3">
</ol>

</details>

<h3>Connecting to Vectors</h3>
<p>Think of the polarization of light as a vector. Each layer of polarized film changes the direction of this vector. By observing the changes in light intensity and direction after each layer, we can visualize how vectors (quantum states) are manipulated in quantum computing.</p>

<img src="https://github.com/LilaShiba/Quantum_computing_lab/assets/13423696/9452116e-fabf-44e4-90ce-3b4bd422b2c4" alt="Explanation In Math">

<h3>Observing Quantum Behavior</h3>
<p>As we pass light through these three layers of polarized film, we observe a phenomenon where the addition of a third filter at a specific angle can allow more light to pass through. Here's how it works:</p>

<ol>
  <li><strong>Polarization Alignment:</strong> The first polarized filter aligns incoming light waves along a specific polarization direction. Only light waves vibrating in this aligned direction can pass through, while others are blocked.</li>

  <li><strong>Further Filtering:</strong> The second filter, oriented at a different angle relative to the first, further restricts the passage of light. It only allows light waves that align with its specific polarization orientation to pass through.</li>

  <li><strong>Introducing the Third Filter:</strong> When we add a third filter at a particular angle relative to the first two, it introduces a new polarization direction. This angle is crucial because it can align with some of the previously blocked light waves that were restricted by the orientations of the first two filters.</li>

  <li><strong>Enhanced Transmission:</strong> As a result, some of the light that was initially blocked by the first two filters can now pass through the third filter. This is because the third filter's angle allows it to transmit light waves that match its polarization orientation, effectively 'unblocking' certain light paths.</li>

  <li><strong>Quantum Analogies:</strong> This behavior resembles quantum superposition, where particles like photons can exist in multiple states simultaneously until observed. In the context of quantum computing, this scenario illustrates how qubits can be manipulated to change their states, akin to how the polarization state of light changes with each additional filter.</li>
</ol>

<p>In essence, the addition of a third polarized filter at a specific angle alters the available paths for light transmission by introducing a new polarization direction that aligns with previously blocked light waves. This phenomenon demonstrates the intricate relationship between polarization angles and light transmission, drawing parallels to quantum principles such as superposition and state manipulation.</p>

<h2>Resources / Works Cited</h2>
<ul>
  <li><a href="https://www.adafruit.com/product/4162">Hardware Setup</a></li>
  <li><a href="https://mitpress.mit.edu/9780262526678/quantum-computing/">Best Book on QC</a></li>
</ul>

</body>
</html>
