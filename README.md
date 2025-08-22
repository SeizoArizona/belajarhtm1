#test-html
sedang belajar bikin website dengan html dan css
[index.html.html](https://github.com/user-attachments/files/21909665/index.html.html)
<<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Learning Dashboard</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        /* Custom CSS for animations and enhancements */
        .card {
            transition: all 0.3s ease;
        }
        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
        }
        .progress-bar {
            transition: width 0.6s ease;
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        .animate-fade {
            animation: fadeIn 0.5s ease-in;
        }
    </style>
</head>
<body class="bg-gray-50">
    <header class="bg-indigo-600 text-white shadow-lg">
        <div class="container mx-auto px-6 py-4">
            <div class="flex items-center justify-between">
                <div class="flex items-center space-x-4">
                    <img src="https://placehold.co/40x40" alt="Learning platform logo showing an open book with a graduation cap" class="rounded-full">
                    <h1 class="text-2xl font-bold">CodeMaster</h1>
                </div>
                <nav>
                    <ul class="flex space-x-6">
                        <li><a href="#" class="hover:text-indigo-200 transition">Home</a></li>
                        <li><a href="#" class="hover:text-indigo-200 transition">Courses</a></li>
                        <li><a href="#" class="hover:text-indigo-200 transition">Projects</a></li>
                        <li><a href="#" class="hover:text-indigo-200 transition">Community</a></li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>

    <main class="container mx-auto px-6 py-8">
        <section class="mb-12 animate-fade">
            <div class="bg-gradient-to-r from-indigo-500 to-purple-600 rounded-xl p-8 text-white">
                <h2 class="text-3xl font-bold mb-4">Welcome to Your Learning Journey</h2>
                <p class="text-lg mb-6">Start coding today with our interactive tutorials and real-world projects.</p>
                <button id="ctaButton" class="bg-white text-indigo-600 px-6 py-3 rounded-lg font-semibold hover:bg-gray-100 transition transform hover:scale-105">
                    Get Started Now
                </button>
            </div>
        </section>

        <section class="mb-12">
            <h2 class="text-2xl font-bold mb-6 border-b pb-2">Learning Paths</h2>
            <div class="grid md:grid-cols-3 gap-6">
                <div class="card bg-white p-6 rounded-xl shadow-md">
                    <div class="flex items-center mb-4">
                        <div class="bg-blue-100 p-3 rounded-lg mr-4">
                            <img src="https://placehold.co/40x40" alt="Python programming language logo with snake icon" class="w-10 h-10">
                        </div>
                        <h3 class="text-xl font-semibold">Python Fundamentals</h3>
                    </div>
                    <p class="text-gray-600 mb-4">Learn Python from scratch with hands-on exercises and projects.</p>
                    <div class="flex justify-between items-center">
                        <div class="w-full bg-gray-200 rounded-full h-2.5">
                            <div class="progress-bar bg-blue-600 h-2.5 rounded-full" style="width: 30%"></div>
                        </div>
                        <span class="text-sm text-gray-500 ml-2">30%</span>
                    </div>
                </div>

                <div class="card bg-white p-6 rounded-xl shadow-md">
                    <div class="flex items-center mb-4">
                        <div class="bg-yellow-100 p-3 rounded-lg mr-4">
                            <img src="https://placehold.co/40x40" alt="JavaScript logo with square brackets and script font" class="w-10 h-10">
                        </div>
                        <h3 class="text-xl font-semibold">Web Development</h3>
                    </div>
                    <p class="text-gray-600 mb-4">Master HTML, CSS and JavaScript to build modern websites.</p>
                    <div class="flex justify-between items-center">
                        <div class="w-full bg-gray-200 rounded-full h-2.5">
                            <div class="progress-bar bg-yellow-500 h-2.5 rounded-full" style="width: 15%"></div>
                        </div>
                        <span class="text-sm text-gray-500 ml-2">15%</span>
                    </div>
                </div>

                <div class="card bg-white p-6 rounded-xl shadow-md">
                    <div class="flex items-center mb-4">
                        <div class="bg-green-100 p-3 rounded-lg mr-4">
                            <img src="https://placehold.co/40x40" alt="Database icon with circular nodes and connections" class="w-10 h-10">
                        </div>
                        <h3 class="text-xl font-semibold">Data Science</h3>
                    </div>
                    <p class="text-gray-600 mb-4">Analyze and visualize data with Python and machine learning.</p>
                    <div class="flex justify-between items-center">
                        <div class="w-full bg-gray-200 rounded-full h-2.5">
                            <div class="progress-bar bg-green-600 h-2.5 rounded-full" style="width: 5%"></div>
                        </div>
                        <span class="text-sm text-gray-500 ml-2">5%</span>
                    </div>
                </div>
            </div>
        </section>

        <section class="mb-12">
            <h2 class="text-2xl font-bold mb-6 border-b pb-2">Coding Challenge</h2>
            <div class="bg-white rounded-xl shadow-md overflow-hidden">
                <div class="md:flex">
                    <div class="md:w-1/2 p-8">
                        <h3 class="text-xl font-semibold mb-4">Temperature Converter</h3>
                        <p class="text-gray-600 mb-6">Build a program that converts between Celsius and Fahrenheit.</p>
                        <div class="space-y-4">
                            <div>
                                <label class="block text-gray-700 mb-2">Value</label>
                                <input type="number" id="tempValue" class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-indigo-500">
                            </div>
                            <div>
                                <label class="block text-gray-700 mb-2">Convert from</label>
                                <select id="fromUnit" class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-indigo-500">
                                    <option value="celsius">Celsius</option>
                                    <option value="fahrenheit">Fahrenheit</option>
                                </select>
                            </div>
                            <button id="convertBtn" class="w-full bg-indigo-600 text-white py-2 rounded-lg hover:bg-indigo-700 transition">
                                Convert
                            </button>
                        </div>
                    </div>
                    <div class="md:w-1/2 bg-gray-50 p-8 flex items-center justify-center">
                        <div class="text-center">
                            <p class="text-gray-500 mb-2">Result</p>
                            <div id="result" class="text-4xl font-bold text-indigo-600">--</div>
                            <div id="resultUnit" class="text-gray-500 mt-2"></div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section>
            <h2 class="text-2xl font-bold mb-6 border-b pb-2">Learning Resources</h2>
            <div class="grid md:grid-cols-2 gap-6">
                <div class="bg-white p-6 rounded-xl shadow-md">
                    <h3 class="text-xl font-semibold mb-3">Documentation Links</h3>
                    <ul class="space-y-2">
                        <li><a href="https://docs.python.org/3/" target="_blank" class="text-indigo-600 hover:underline">Python Official Docs</a></li>
                        <li><a href="https://developer.mozilla.org/en-US/" target="_blank" class="text-indigo-600 hover:underline">MDN Web Docs</a></li>
                        <li><a href="https://www.w3schools.com/" target="_blank" class="text-indigo-600 hover:underline">W3Schools</a></li>
                    </ul>
                </div>
                <div class="bg-white p-6 rounded-xl shadow-md">
                    <h3 class="text-xl font-semibold mb-3">Learning Tips</h3>
                    <ol class="list-decimal pl-5 space-y-2">
                        <li>Practice coding daily, even for just 30 minutes</li>
                        <li>Build small projects to apply what you learn</li>
                        <li>Don't hesitate to make mistakes - they're part of learning</li>
                        <li>Join coding communities for support and inspiration</li>
                    </ol>
                </div>
            </div>
        </section>
    </main>

    <footer class="bg-gray-800 text-white py-8">
        <div class="container mx-auto px-6">
            <div class="flex flex-col md:flex-row justify-between">
                <div class="mb-6 md:mb-0">
                    <h3 class="text-xl font-bold mb-4">CodeMaster</h3>
                    <p class="text-gray-400">Empowering your coding journey since 2023.</p>
                </div>
                <div>
                    <h4 class="text-lg font-semibold mb-3">Quick Links</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white transition">About Us</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Contact</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Privacy Policy</a></li>
                    </ul>
                </div>
            </div>
            <div class="border-t border-gray-700 mt-8 pt-6 text-center text-gray-400">
                <p>© 2023 CodeMaster. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <script>
        // Temperature Converter Functionality
        document.getElementById('convertBtn').addEventListener('click', function() {
            const value = parseFloat(document.getElementById('tempValue').value);
            const fromUnit = document.getElementById('fromUnit').value;
            let result, resultUnit;

            if (isNaN(value)) {
                alert('Please enter a valid number');
                return;
            }

            if (fromUnit === 'celsius') {
                result = (value * 9/5) + 32;
                resultUnit = 'Fahrenheit';
            } else {
                result = (value - 32) * 5/9;
                resultUnit = 'Celsius';
            }

            document.getElementById('result').textContent = result.toFixed(1);
            document.getElementById('resultUnit').textContent = resultUnit;
        });

        // CTA Button Animation
        document.getElementById('ctaButton').addEventListener('mouseenter', function() {
            this.classList.add('animate-pulse');
        });

        document.getElementById('ctaButton').addEventListener('mouseleave', function() {
            this.classList.remove('animate-pulse');
        });

        // Simulate progress bar animation on page load
        document.addEventListener('DOMContentLoaded', function() {
            const progressBars = document.querySelectorAll('.progress-bar');
            progressBars.forEach(bar => {
                // Reset to 0 for animation effect
                const targetWidth = bar.style.width;
                bar.style.width = '0';
                setTimeout(() => {
                    bar.style.width = targetWidth;
                }, 300);
            });
        });
    </script>
</body>
</html>



<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Learning Dashboard</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        /* Custom CSS for animations and enhancements */
        .card {
            transition: all 0.3s ease;
        }
        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
        }
        .progress-bar {
            transition: width 0.6s ease;
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        .animate-fade {
            animation: fadeIn 0.5s ease-in;
        }
    </style>
</head>
<body class="bg-gray-50">
    <header class="bg-indigo-600 text-white shadow-lg">
        <div class="container mx-auto px-6 py-4">
            <div class="flex items-center justify-between">
                <div class="flex items-center space-x-4">
                    <img src="https://placehold.co/40x40" alt="Learning platform logo showing an open book with a graduation cap" class="rounded-full">
                    <h1 class="text-2xl font-bold">CodeMaster</h1>
                </div>
                <nav>
                    <ul class="flex space-x-6">
                        <li><a href="#" class="hover:text-indigo-200 transition">Home</a></li>
                        <li><a href="#" class="hover:text-indigo-200 transition">Courses</a></li>
                        <li><a href="#" class="hover:text-indigo-200 transition">Projects</a></li>
                        <li><a href="#" class="hover:text-indigo-200 transition">Community</a></li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>

    <main class="container mx-auto px-6 py-8">
        <section class="mb-12 animate-fade">
            <div class="bg-gradient-to-r from-indigo-500 to-purple-600 rounded-xl p-8 text-white">
                <h2 class="text-3xl font-bold mb-4">Welcome to Your Learning Journey</h2>
                <p class="text-lg mb-6">Start coding today with our interactive tutorials and real-world projects.</p>
                <button id="ctaButton" class="bg-white text-indigo-600 px-6 py-3 rounded-lg font-semibold hover:bg-gray-100 transition transform hover:scale-105">
                    Get Started Now
                </button>
            </div>
        </section>

        <section class="mb-12">
            <h2 class="text-2xl font-bold mb-6 border-b pb-2">Learning Paths</h2>
            <div class="grid md:grid-cols-3 gap-6">
                <div class="card bg-white p-6 rounded-xl shadow-md">
                    <div class="flex items-center mb-4">
                        <div class="bg-blue-100 p-3 rounded-lg mr-4">
                            <img src="https://placehold.co/40x40" alt="Python programming language logo with snake icon" class="w-10 h-10">
                        </div>
                        <h3 class="text-xl font-semibold">Python Fundamentals</h3>
                    </div>
                    <p class="text-gray-600 mb-4">Learn Python from scratch with hands-on exercises and projects.</p>
                    <div class="flex justify-between items-center">
                        <div class="w-full bg-gray-200 rounded-full h-2.5">
                            <div class="progress-bar bg-blue-600 h-2.5 rounded-full" style="width: 30%"></div>
                        </div>
                        <span class="text-sm text-gray-500 ml-2">30%</span>
                    </div>
                </div>

                <div class="card bg-white p-6 rounded-xl shadow-md">
                    <div class="flex items-center mb-4">
                        <div class="bg-yellow-100 p-3 rounded-lg mr-4">
                            <img src="https://placehold.co/40x40" alt="JavaScript logo with square brackets and script font" class="w-10 h-10">
                        </div>
                        <h3 class="text-xl font-semibold">Web Development</h3>
                    </div>
                    <p class="text-gray-600 mb-4">Master HTML, CSS and JavaScript to build modern websites.</p>
                    <div class="flex justify-between items-center">
                        <div class="w-full bg-gray-200 rounded-full h-2.5">
                            <div class="progress-bar bg-yellow-500 h-2.5 rounded-full" style="width: 15%"></div>
                        </div>
                        <span class="text-sm text-gray-500 ml-2">15%</span>
                    </div>
                </div>

                <div class="card bg-white p-6 rounded-xl shadow-md">
                    <div class="flex items-center mb-4">
                        <div class="bg-green-100 p-3 rounded-lg mr-4">
                            <img src="https://placehold.co/40x40" alt="Database icon with circular nodes and connections" class="w-10 h-10">
                        </div>
                        <h3 class="text-xl font-semibold">Data Science</h3>
                    </div>
                    <p class="text-gray-600 mb-4">Analyze and visualize data with Python and machine learning.</p>
                    <div class="flex justify-between items-center">
                        <div class="w-full bg-gray-200 rounded-full h-2.5">
                            <div class="progress-bar bg-green-600 h-2.5 rounded-full" style="width: 5%"></div>
                        </div>
                        <span class="text-sm text-gray-500 ml-2">5%</span>
                    </div>
                </div>
            </div>
        </section>

        <section class="mb-12">
            <h2 class="text-2xl font-bold mb-6 border-b pb-2">Coding Challenge</h2>
            <div class="bg-white rounded-xl shadow-md overflow-hidden">
                <div class="md:flex">
                    <div class="md:w-1/2 p-8">
                        <h3 class="text-xl font-semibold mb-4">Temperature Converter</h3>
                        <p class="text-gray-600 mb-6">Build a program that converts between Celsius and Fahrenheit.</p>
                        <div class="space-y-4">
                            <div>
                                <label class="block text-gray-700 mb-2">Value</label>
                                <input type="number" id="tempValue" class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-indigo-500">
                            </div>
                            <div>
                                <label class="block text-gray-700 mb-2">Convert from</label>
                                <select id="fromUnit" class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-indigo-500">
                                    <option value="celsius">Celsius</option>
                                    <option value="fahrenheit">Fahrenheit</option>
                                </select>
                            </div>
                            <button id="convertBtn" class="w-full bg-indigo-600 text-white py-2 rounded-lg hover:bg-indigo-700 transition">
                                Convert
                            </button>
                        </div>
                    </div>
                    <div class="md:w-1/2 bg-gray-50 p-8 flex items-center justify-center">
                        <div class="text-center">
                            <p class="text-gray-500 mb-2">Result</p>
                            <div id="result" class="text-4xl font-bold text-indigo-600">--</div>
                            <div id="resultUnit" class="text-gray-500 mt-2"></div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section>
            <h2 class="text-2xl font-bold mb-6 border-b pb-2">Learning Resources</h2>
            <div class="grid md:grid-cols-2 gap-6">
                <div class="bg-white p-6 rounded-xl shadow-md">
                    <h3 class="text-xl font-semibold mb-3">Documentation Links</h3>
                    <ul class="space-y-2">
                        <li><a href="https://docs.python.org/3/" target="_blank" class="text-indigo-600 hover:underline">Python Official Docs</a></li>
                        <li><a href="https://developer.mozilla.org/en-US/" target="_blank" class="text-indigo-600 hover:underline">MDN Web Docs</a></li>
                        <li><a href="https://www.w3schools.com/" target="_blank" class="text-indigo-600 hover:underline">W3Schools</a></li>
                    </ul>
                </div>
                <div class="bg-white p-6 rounded-xl shadow-md">
                    <h3 class="text-xl font-semibold mb-3">Learning Tips</h3>
                    <ol class="list-decimal pl-5 space-y-2">
                        <li>Practice coding daily, even for just 30 minutes</li>
                        <li>Build small projects to apply what you learn</li>
                        <li>Don't hesitate to make mistakes - they're part of learning</li>
                        <li>Join coding communities for support and inspiration</li>
                    </ol>
                </div>
            </div>
        </section>
    </main>

    <footer class="bg-gray-800 text-white py-8">
        <div class="container mx-auto px-6">
            <div class="flex flex-col md:flex-row justify-between">
                <div class="mb-6 md:mb-0">
                    <h3 class="text-xl font-bold mb-4">CodeMaster</h3>
                    <p class="text-gray-400">Empowering your coding journey since 2023.</p>
                </div>
                <div>
                    <h4 class="text-lg font-semibold mb-3">Quick Links</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white transition">About Us</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Contact</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Privacy Policy</a></li>
                    </ul>
                </div>
            </div>
            <div class="border-t border-gray-700 mt-8 pt-6 text-center text-gray-400">
                <p>© 2023 CodeMaster. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <script>
        // Temperature Converter Functionality
        document.getElementById('convertBtn').addEventListener('click', function() {
            const value = parseFloat(document.getElementById('tempValue').value);
            const fromUnit = document.getElementById('fromUnit').value;
            let result, resultUnit;

            if (isNaN(value)) {
                alert('Please enter a valid number');
                return;
            }

            if (fromUnit === 'celsius') {
                result = (value * 9/5) + 32;
                resultUnit = 'Fahrenheit';
            } else {
                result = (value - 32) * 5/9;
                resultUnit = 'Celsius';
            }

            document.getElementById('result').textContent = result.toFixed(1);
            document.getElementById('resultUnit').textContent = resultUnit;
        });

        // CTA Button Animation
        document.getElementById('ctaButton').addEventListener('mouseenter', function() {
            this.classList.add('animate-pulse');
        });

        document.getElementById('ctaButton').addEventListener('mouseleave', function() {
            this.classList.remove('animate-pulse');
        });

        // Simulate progress bar animation on page load
        document.addEventListener('DOMContentLoaded', function() {
            const progressBars = document.querySelectorAll('.progress-bar');
            progressBars.forEach(bar => {
                // Reset to 0 for animation effect
                const targetWidth = bar.style.width;
                bar.style.width = '0';
                setTimeout(() => {
                    bar.style.width = targetWidth;
                }, 300);
            });
        });
    </script>
</body>
</html>
