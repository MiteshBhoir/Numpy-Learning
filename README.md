<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Numpy Fundamentals and Exercises</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #0d1117; /* GitHub Dark Background */
            color: #c9d1d9; /* Light Text */
        }
        .code-block {
            background-color: #161b22; /* Slightly darker background for code */
            border: 1px solid #30363d;
            border-radius: 8px;
            position: relative;
            padding: 1rem;
            margin-top: 0.75rem;
            overflow-x: auto;
        }
        /* Custom scrollbar for webkit browsers for table/code overflow */
        .table-container::-webkit-scrollbar, .code-block::-webkit-scrollbar {
            height: 6px;
        }
        .table-container::-webkit-scrollbar-thumb, .code-block::-webkit-scrollbar-thumb {
            background: #30363d;
            border-radius: 3px;
        }
        .table-container::-webkit-scrollbar-track, .code-block::-webkit-scrollbar-track {
            background: #0d1117;
        }
    </style>
</head>
<body class="p-4 sm:p-8">

    <div class="max-w-4xl mx-auto">
        <!-- Header -->
        <header class="mb-8 p-4 bg-gray-800 rounded-xl shadow-lg border border-gray-700">
            <h1 class="text-4xl font-bold mb-2 flex items-center text-blue-400">
                <span class="mr-3">📊</span> Numpy Fundamentals and Exercises
            </h1>
            <p class="text-gray-400 text-lg">
                This repository contains a collection of Jupyter Notebooks dedicated to learning, demonstrating, and practicing core concepts and advanced techniques of the **NumPy** library in Python.
            </p>
            <p class="mt-2 text-sm text-gray-500">
                NumPy is the fundamental package for scientific computing in Python.
            </p>
        </header>

        <!-- Repository Contents -->
        <section class="mb-12">
            <h2 class="text-2xl font-semibold mb-4 border-b border-gray-700 pb-2 flex items-center text-green-400">
                <span class="mr-2">📂</span> Repository Contents
            </h2>
            <p class="mb-4 text-gray-400">The repository is structured around progressive learning modules and practical exercises:</p>

            <div class="table-container overflow-x-auto rounded-lg border border-gray-700">
                <table class="min-w-full divide-y divide-gray-700">
                    <thead class="bg-gray-700">
                        <tr>
                            <th scope="col" class="px-6 py-3 text-left text-xs font-medium uppercase tracking-wider">File Name</th>
                            <th scope="col" class="px-6 py-3 text-left text-xs font-medium uppercase tracking-wider">Description</th>
                            <th scope="col" class="px-6 py-3 text-left text-xs font-medium uppercase tracking-wider">Key Topics Covered</th>
                        </tr>
                    </thead>
                    <tbody class="divide-y divide-gray-800">
                        <tr class="hover:bg-gray-800 transition duration-150">
                            <td class="px-6 py-4 whitespace-nowrap font-mono text-sm text-yellow-300">numpy_1.ipynb</td>
                            <td class="px-6 py-4 text-sm text-gray-300">Numpy Basics and Array Attributes</td>
                            <td class="px-6 py-4 text-sm text-gray-400">Creation of arrays from lists, array generation functions, random array creation, attributes (`shape`, `size`, `dtype`, etc.), basic array methods, and **Reshaping**.</td>
                        </tr>
                        <tr class="hover:bg-gray-800 transition duration-150">
                            <td class="px-6 py-4 whitespace-nowrap font-mono text-sm text-yellow-300">Numpy_2_indexing.ipynb</td>
                            <td class="px-6 py-4 text-sm text-gray-300">Advanced Indexing, Slicing, and Operations</td>
                            <td class="px-6 py-4 text-sm text-gray-400">Indexing/slicing (1D/2D), **Boolean Indexing**, array arithmetic, **Broadcasting**, **Deep/Shallow Copy**, matrix operations, and array stacking/splitting.</td>
                        </tr>
                        <tr class="hover:bg-gray-800 transition duration-150">
                            <td class="px-6 py-4 whitespace-nowrap font-mono text-sm text-yellow-300">exersises .ipynb</td>
                            <td class="px-6 py-4 text-sm text-gray-300">Practical Numpy Exercises</td>
                            <td class="px-6 py-4 text-sm text-gray-400">Sudoku validation challenge, student data manipulation (averages, filtering, updates).</td>
                        </tr>
                    </tbody>
                </table>
            </div>
        </section>

        <!-- Prerequisites -->
        <section class="mb-12">
            <h2 class="text-2xl font-semibold mb-4 border-b border-gray-700 pb-2 flex items-center text-red-400">
                <span class="mr-2">🛠️</span> Prerequisites
            </h2>
            <p class="mb-4 text-gray-400">To run these notebooks locally, you need:</p>
            <ul class="list-disc list-inside space-y-2 ml-4 text-gray-300">
                <li>**Python** (version 3.6+)</li>
                <li>**Jupyter Notebook** or **JupyterLab** (or a compatible environment like Google Colab).</li>
                <li>The **NumPy** library.</li>
            </ul>

            <h3 class="text-xl font-medium mt-6 mb-2 text-gray-200">Installation</h3>
            <div class="code-container relative">
                <pre id="code-install" class="code-block font-mono text-sm">pip install numpy</pre>
                <button class="copy-btn absolute top-3 right-3 text-xs px-2 py-1 bg-blue-600 hover:bg-blue-700 text-white rounded-md transition duration-150" data-target="code-install">Copy</button>
            </div>
        </section>

        <!-- Getting Started -->
        <section class="mb-12">
            <h2 class="text-2xl font-semibold mb-4 border-b border-gray-700 pb-2 flex items-center text-yellow-400">
                <span class="mr-2">🚀</span> Getting Started
            </h2>
            <ol class="list-decimal list-inside space-y-4 ml-4 text-gray-300">
                <li>
                    <p class="font-semibold">Clone the repository:</p>
                    <div class="code-container relative ml-4 mt-1">
                        <pre id="code-clone" class="code-block font-mono text-sm">git clone https://github.com/MiteshBhoir/Numpy-Learning.git</pre>
                        <button class="copy-btn absolute top-3 right-3 text-xs px-2 py-1 bg-blue-600 hover:bg-blue-700 text-white rounded-md transition duration-150" data-target="code-clone">Copy</button>
                    </div>
                </li>
                <li>
                    <p class="font-semibold">Navigate to the directory:</p>
                    <div class="code-container relative ml-4 mt-1">
                        <pre id="code-cd" class="code-block font-mono text-sm">cd Numpy-Learning</pre>
                        <button class="copy-btn absolute top-3 right-3 text-xs px-2 py-1 bg-blue-600 hover:bg-blue-700 text-white rounded-md transition duration-150" data-target="code-cd">Copy</button>
                    </div>
                </li>
                <li>
                    <p class="font-semibold">Launch Jupyter Notebook/Lab:</p>
                    <div class="code-container relative ml-4 mt-1">
                        <pre id="code-launch" class="code-block font-mono text-sm">jupyter notebook</pre>
                        <button class="copy-btn absolute top-3 right-3 text-xs px-2 py-1 bg-blue-600 hover:bg-blue-700 text-white rounded-md transition duration-150" data-target="code-launch">Copy</button>
                    </div>
                </li>
            </ol>
            <p class="mt-4 ml-4 text-gray-400">Click on any of the `.ipynb` files to start learning and executing the code!</p>
        </section>

        <!-- How to Use -->
        <section class="mb-8">
            <h2 class="text-2xl font-semibold mb-4 border-b border-gray-700 pb-2 flex items-center text-indigo-400">
                <span class="mr-2">💡</span> How to Use
            </h2>
            <ul class="list-none space-y-3 text-gray-300">
                <li class="p-3 bg-gray-800 rounded-lg border border-gray-700">
                    <span class="font-bold text-lg text-blue-300">For Beginners:</span> Start with <code class="font-mono text-yellow-300">numpy_1.ipynb</code> to build a solid foundation on array creation and attributes.
                </li>
                <li class="p-3 bg-gray-800 rounded-lg border border-gray-700">
                    <span class="font-bold text-lg text-green-300">Intermediate Users:</span> Move to <code class="font-mono text-yellow-300">Numpy_2_indexing.ipynb</code> to master powerful techniques like slicing, boolean indexing, and copying.
                </li>
                <li class="p-3 bg-gray-800 rounded-lg border border-gray-700">
                    <span class="font-bold text-lg text-red-300">Practice:</span> Use <code class="font-mono text-yellow-300">exersises .ipynb</code> to test your knowledge against real-world data manipulation and logic problems.
                </li>
            </ul>
        </section>

        <footer class="text-center mt-12 pt-6 border-t border-gray-700 text-gray-500">
            Enjoy your journey into scientific computing with NumPy!
        </footer>
    </div>

    <!-- JavaScript for Copy Functionality -->
    <script>
        document.querySelectorAll('.copy-btn').forEach(button => {
            button.addEventListener('click', (event) => {
                const targetId = event.currentTarget.getAttribute('data-target');
                const targetElement = document.getElementById(targetId);

                if (targetElement) {
                    // Get the text content, removing leading/trailing whitespace
                    const textToCopy = targetElement.textContent.trim();

                    // Use a temporary textarea for copying (works reliably in sandboxed environments)
                    const textarea = document.createElement('textarea');
                    textarea.value = textToCopy;
                    document.body.appendChild(textarea);
                    textarea.select();

                    try {
                        document.execCommand('copy');
                        
                        // Provide feedback to the user
                        const originalText = event.currentTarget.textContent;
                        event.currentTarget.textContent = 'Copied!';
                        event.currentTarget.classList.add('bg-green-600', 'hover:bg-green-600');
                        event.currentTarget.classList.remove('bg-blue-600', 'hover:bg-blue-700');

                        setTimeout(() => {
                            event.currentTarget.textContent = originalText;
                            event.currentTarget.classList.remove('bg-green-600', 'hover:bg-green-600');
                            event.currentTarget.classList.add('bg-blue-600', 'hover:bg-blue-700');
                        }, 1500);

                    } catch (err) {
                        console.error('Could not copy text: ', err);
                    } finally {
                        document.body.removeChild(textarea);
                    }
                }
            });
        });
    </script>
</body>
</html>
