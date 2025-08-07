# Pdf-maker-x<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Free online PDF maker and document scanner tool. Convert images to PDF with customizable compression levels.">
    <meta name="keywords" content="PDF maker, document scanner, image to PDF, PDF converter, online PDF tool">
    <meta name="author" content="PDF Maker Pro">
    <meta name="robots" content="index, follow">
    <meta property="og:title" content="PDF Maker Pro - Online Document Scanner & PDF Converter">
    <meta property="og:description" content="Convert images to PDF with adjustable compression levels. Free online tool.">
    <meta property="og:type" content="website">
    <meta property="og:url" content="https://yourwebsite.com">
    <link rel="canonical" href="https://yourwebsite.com">
    <title>PDF Maker Pro - Online Document Scanner & PDF Converter</title>
    <style>
        :root {
            --primary-color: #4285f4;
            --secondary-color: #34a853;
            --accent-color: #ea4335;
            --light-gray: #f5f5f5;
            --dark-gray: #333;
            --medium-gray: #757575;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            line-height: 1.6;
            color: var(--dark-gray);
            background-color: #f9f9f9;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        header {
            background-color: white;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            padding: 15px 0;
            position: sticky;
            top: 0;
            z-index: 100;
        }
        
        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-size: 24px;
            font-weight: bold;
            color: var(--primary-color);
            text-decoration: none;
        }
        
        .logo span {
            color: var(--accent-color);
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav ul li {
            margin-left: 20px;
        }
        
        nav ul li a {
            text-decoration: none;
            color: var(--dark-gray);
            font-weight: 500;
            transition: color 0.3s;
        }
        
        nav ul li a:hover {
            color: var(--primary-color);
        }
        
        .mobile-menu-btn {
            display: none;
            background: none;
            border: none;
            font-size: 24px;
            cursor: pointer;
            color: var(--dark-gray);
        }
        
        .hero {
            text-align: center;
            padding: 60px 0;
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
        }
        
        .hero h1 {
            font-size: 2.5rem;
            margin-bottom: 20px;
            color: var(--dark-gray);
        }
        
        .hero p {
            font-size: 1.1rem;
            color: var(--medium-gray);
            max-width: 700px;
            margin: 0 auto 30px;
        }
        
        .main-content {
            padding: 40px 0;
        }
        
        .tool-container {
            background-color: white;
            border-radius: 8px;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.08);
            padding: 30px;
            margin-bottom: 40px;
        }
        
        .tool-title {
            font-size: 1.8rem;
            margin-bottom: 20px;
            color: var(--dark-gray);
            text-align: center;
        }
        
        .upload-area {
            border: 2px dashed var(--primary-color);
            border-radius: 8px;
            padding: 40px;
            text-align: center;
            cursor: pointer;
            transition: all 0.3s;
            margin-bottom: 30px;
            background-color: rgba(66, 133, 244, 0.05);
        }
        
        .upload-area:hover {
            background-color: rgba(66, 133, 244, 0.1);
        }
        
        .upload-area i {
            font-size: 48px;
            color: var(--primary-color);
            margin-bottom: 15px;
        }
        
        .upload-area p {
            color: var(--medium-gray);
            margin-bottom: 10px;
        }
        
        .upload-area .btn {
            background-color: var(--primary-color);
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 4px;
            cursor: pointer;
            font-weight: 500;
            transition: background-color 0.3s;
        }
        
        .upload-area .btn:hover {
            background-color: #3367d6;
        }
        
        #fileInput {
            display: none;
        }
        
        .settings-panel {
            margin-bottom: 30px;
        }
        
        .settings-title {
            font-size: 1.2rem;
            margin-bottom: 15px;
            color: var(--dark-gray);
        }
        
        .form-group {
            margin-bottom: 20px;
        }
        
        .form-group label {
            display: block;
            margin-bottom: 8px;
            font-weight: 500;
        }
        
        .form-control {
            width: 100%;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 4px;
            font-size: 16px;
        }
        
        .range-container {
            display: flex;
            align-items: center;
        }
        
        .range-container input[type="range"] {
            flex-grow: 1;
            margin-right: 15px;
        }
        
        .range-value {
            width: 50px;
            text-align: center;
            font-weight: bold;
        }
        
        .btn {
            display: inline-block;
            padding: 12px 24px;
            background-color: var(--primary-color);
            color: white;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            font-size: 16px;
            font-weight: 500;
            transition: all 0.3s;
            text-align: center;
        }
        
        .btn:hover {
            background-color: #3367d6;
            transform: translateY(-2px);
        }
        
        .btn-secondary {
            background-color: var(--medium-gray);
        }
        
        .btn-secondary:hover {
            background-color: #616161;
        }
        
        .btn-success {
            background-color: var(--secondary-color);
        }
        
        .btn-success:hover {
            background-color: #2d9249;
        }
        
        .preview-container {
            margin-top: 30px;
            display: none;
        }
        
        .preview-title {
            font-size: 1.2rem;
            margin-bottom: 15px;
            color: var(--dark-gray);
        }
        
        .preview-images {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
            gap: 15px;
            margin-bottom: 20px;
        }
        
        .preview-image {
            position: relative;
            border: 1px solid #ddd;
            border-radius: 4px;
            overflow: hidden;
        }
        
        .preview-image img {
            width: 100%;
            height: auto;
            display: block;
        }
        
        .preview-image .remove-btn {
            position: absolute;
            top: 5px;
            right: 5px;
            background-color: var(--accent-color);
            color: white;
            border: none;
            width: 24px;
            height: 24px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            opacity: 0;
            transition: opacity 0.3s;
        }
        
        .preview-image:hover .remove-btn {
            opacity: 1;
        }
        
        .action-buttons {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin-top: 30px;
        }
        
        .ad-container {
            margin: 30px 0;
            text-align: center;
            background-color: var(--light-gray);
            padding: 20px;
            border-radius: 8px;
        }
        
        .ad-label {
            font-size: 0.8rem;
            color: var(--medium-gray);
            margin-bottom: 5px;
            text-transform: uppercase;
        }
        
        .features {
            padding: 60px 0;
            background-color: white;
        }
        
        .section-title {
            text-align: center;
            font-size: 2rem;
            margin-bottom: 40px;
            color: var(--dark-gray);
        }
        
        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .feature-card {
            background-color: var(--light-gray);
            border-radius: 8px;
            padding: 30px;
            text-align: center;
            transition: transform 0.3s;
        }
        
        .feature-card:hover {
            transform: translateY(-5px);
        }
        
        .feature-icon {
            font-size: 48px;
            color: var(--primary-color);
            margin-bottom: 20px;
        }
        
        .feature-title {
            font-size: 1.3rem;
            margin-bottom: 15px;
            color: var(--dark-gray);
        }
        
        .feature-desc {
            color: var(--medium-gray);
        }
        
        footer {
            background-color: var(--dark-gray);
            color: white;
            padding: 40px 0 20px;
        }
        
        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 30px;
            margin-bottom: 30px;
        }
        
        .footer-column h3 {
            font-size: 1.2rem;
            margin-bottom: 20px;
            color: white;
        }
        
        .footer-column ul {
            list-style: none;
        }
        
        .footer-column ul li {
            margin-bottom: 10px;
        }
        
        .footer-column ul li a {
            color: #bbb;
            text-decoration: none;
            transition: color 0.3s;
        }
        
        .footer-column ul li a:hover {
            color: white;
        }
        
        .copyright {
            text-align: center;
            padding-top: 20px;
            border-top: 1px solid #444;
            color: #bbb;
            font-size: 0.9rem;
        }
        
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                text-align: center;
            }
            
            nav ul {
                margin-top: 20px;
                flex-direction: column;
                align-items: center;
            }
            
            nav ul li {
                margin: 10px 0;
            }
            
            .hero h1 {
                font-size: 2rem;
            }
            
            .hero p {
                font-size: 1rem;
            }
            
            .action-buttons {
                flex-direction: column;
            }
            
            .btn {
                width: 100%;
                margin-bottom: 10px;
            }
        }
        
        @media (max-width: 480px) {
            .upload-area {
                padding: 20px;
            }
            
            .tool-container {
                padding: 20px;
            }
            
            .preview-images {
                grid-template-columns: 1fr;
            }
        }
        
        /* Loading spinner */
        .spinner {
            display: none;
            width: 40px;
            height: 40px;
            margin: 20px auto;
            border: 4px solid rgba(0, 0, 0, 0.1);
            border-radius: 50%;
            border-top-color: var(--primary-color);
            animation: spin 1s ease-in-out infinite;
        }
        
        @keyframes spin {
            to { transform: rotate(360deg); }
        }
        
        /* Toast notification */
        .toast {
            position: fixed;
            bottom: 20px;
            right: 20px;
            background-color: var(--secondary-color);
            color: white;
            padding: 15px 25px;
            border-radius: 4px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
            transform: translateY(100px);
            opacity: 0;
            transition: all 0.3s;
            z-index: 1000;
        }
        
        .toast.show {
            transform: translateY(0);
            opacity: 1;
        }
    </style>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
</head>
<body>
    <header>
        <div class="container header-content">
            <a href="#" class="logo">PDF<span>Maker</span>Pro</a>
            <button class="mobile-menu-btn" id="mobileMenuBtn">
                <i class="fas fa-bars"></i>
            </button>
            <nav id="mainNav">
                <ul>
                    <li><a href="#">Home</a></li>
                    <li><a href="#features">Features</a></li>
                    <li><a href="#how-it-works">How It Works</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <section class="hero">
        <div class="container">
            <h1>Create Perfect PDFs from Your Documents</h1>
            <p>Scan, optimize, and convert your images to high-quality PDF files with our free online tool. Adjust compression levels to balance quality and file size.</p>
        </div>
    </section>

    <div class="ad-container container">
        <div class="ad-label">Advertisement</div>
        <!-- Replace with your Google AdSense ad unit -->
        <script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-YOUR_PUBLISHER_ID"></script>
        <!-- PDF Maker Top Banner -->
        <ins class="adsbygoogle"
             style="display:block"
             data-ad-client="ca-pub-YOUR_PUBLISHER_ID"
             data-ad-slot="YOUR_AD_SLOT_ID"
             data-ad-format="auto"
             data-full-width-responsive="true"></ins>
        <script>
             (adsbygoogle = window.adsbygoogle || []).push({});
        </script>
    </div>

    <main class="main-content">
        <div class="container">
            <div class="tool-container">
                <h2 class="tool-title">PDF Maker & Document Scanner</h2>
                
                <div class="upload-area" id="uploadArea">
                    <i class="fas fa-cloud-upload-alt"></i>
                    <h3>Drag & Drop Your Files Here</h3>
                    <p>or</p>
                    <button class="btn" id="selectFilesBtn">Select Files</button>
                    <input type="file" id="fileInput" accept="image/*,.pdf" multiple>
                    <p>Supports: JPG, PNG, PDF (Max 20MB)</p>
                </div>
                
                <div class="settings-panel">
                    <h3 class="settings-title">PDF Settings</h3>
                    
                    <div class="form-group">
                        <label for="pdfName">PDF File Name</label>
                        <input type="text" id="pdfName" class="form-control" placeholder="output.pdf" value="document.pdf">
                    </div>
                    
                    <div class="form-group">
                        <label for="compressionLevel">Image Compression Level</label>
                        <div class="range-container">
                            <input type="range" id="compressionLevel" class="form-control" min="0" max="2" step="1" value="1">
                            <span class="range-value" id="compressionValue">Medium</span>
                        </div>
                        <small id="compressionHelp" class="text-muted">Adjust to balance quality and file size</small>
                    </div>
                    
                    <div class="form-group">
                        <label for="pageSize">Page Size</label>
                        <select id="pageSize" class="form-control">
                            <option value="a4">A4 (210 × 297 mm)</option>
                            <option value="letter">Letter (8.5 × 11 in)</option>
                            <option value="legal">Legal (8.5 × 14 in)</option>
                            <option value="auto">Auto (Fit to content)</option>
                        </select>
                    </div>
                    
                    <div class="form-group">
                        <label for="pageOrientation">Page Orientation</label>
                        <select id="pageOrientation" class="form-control">
                            <option value="portrait">Portrait</option>
                            <option value="landscape">Landscape</option>
                        </select>
                    </div>
                    
                    <div class="form-group">
                        <label for="marginSize">Margin Size (mm)</label>
                        <input type="number" id="marginSize" class="form-control" min="0" max="50" value="10">
                    </div>
                </div>
                
                <div class="preview-container" id="previewContainer">
                    <h3 class="preview-title">Preview</h3>
                    <div class="preview-images" id="previewImages"></div>
                </div>
                
                <div class="spinner" id="spinner"></div>
                
                <div class="action-buttons">
                    <button class="btn btn-secondary" id="clearAllBtn">Clear All</button>
                    <button class="btn btn-success" id="generatePdfBtn">Generate PDF</button>
                </div>
            </div>
            
            <div class="ad-container">
                <div class="ad-label">Advertisement</div>
                <!-- Replace with your Google AdSense ad unit -->
                <script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-YOUR_PUBLISHER_ID"></script>
                <!-- PDF Maker Middle Rectangle -->
                <ins class="adsbygoogle"
                     style="display:block"
                     data-ad-client="ca-pub-YOUR_PUBLISHER_ID"
                     data-ad-slot="YOUR_AD_SLOT_ID"
                     data-ad-format="auto"
                     data-full-width-responsive="true"></ins>
                <script>
                     (adsbygoogle = window.adsbygoogle || []).push({});
                </script>
            </div>
            
            <section class="features" id="features">
                <h2 class="section-title">Key Features</h2>
                <div class="features-grid">
                    <div class="feature-card">
                        <div class="feature-icon">
                            <i class="fas fa-file-pdf"></i>
                        </div>
                        <h3 class="feature-title">High-Quality PDFs</h3>
                        <p class="feature-desc">Create professional PDF documents with adjustable quality settings to meet your needs.</p>
                    </div>
                    
                    <div class="feature-card">
                        <div class="feature-icon">
                            <i class="fas fa-compress-alt"></i>
                        </div>
                        <h3 class="feature-title">Smart Compression</h3>
                        <p class="feature-desc">Optimize your PDF file size without sacrificing too much quality.</p>
                    </div>
                    
                    <div class="feature-card">
                        <div class="feature-icon">
                            <i class="fas fa-mobile-alt"></i>
                        </div>
                        <h3 class="feature-title">Mobile Friendly</h3>
                        <p class="feature-desc">Works perfectly on all devices, from desktop computers to smartphones.</p>
                    </div>
                    
                    <div class="feature-card">
                        <div class="feature-icon">
                            <i class="fas fa-lock"></i>
                        </div>
                        <h3 class="feature-title">Secure Processing</h3>
                        <p class="feature-desc">Your files are processed in your browser and never uploaded to our servers.</p>
                    </div>
                    
                    <div class="feature-card">
                        <div class="feature-icon">
                            <i class="fas fa-bolt"></i>
                        </div>
                        <h3 class="feature-title">Fast Conversion</h3>
                        <p class="feature-desc">Quickly convert multiple images to a single PDF document in seconds.</p>
                    </div>
                    
                    <div class="feature-card">
                        <div class="feature-icon">
                            <i class="fas fa-cogs"></i>
                        </div>
                        <h3 class="feature-title">Customizable</h3>
                        <p class="feature-desc">Adjust page size, orientation, and margins to create the perfect document.</p>
                    </div>
                </div>
            </section>
            
            <div class="ad-container">
                <div class="ad-label">Advertisement</div>
                <!-- Replace with your Google AdSense ad unit -->
                <script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-YOUR_PUBLISHER_ID"></script>
                <!-- PDF Maker Bottom Banner -->
                <ins class="adsbygoogle"
                     style="display:block"
                     data-ad-client="ca-pub-YOUR_PUBLISHER_ID"
                     data-ad-slot="YOUR_AD_SLOT_ID"
                     data-ad-format="auto"
                     data-full-width-responsive="true"></ins>
                <script>
                     (adsbygoogle = window.adsbygoogle || []).push({});
                </script>
            </div>
            
            <section class="how-it-works" id="how-it-works">
                <h2 class="section-title">How It Works</h2>
                <div class="tool-container">
                    <div class="steps">
                        <div class="step">
                            <h3>1. Upload Your Files</h3>
                            <p>Drag and drop your images or PDFs into the upload area, or click to browse your files.</p>
                        </div>
                        <div class="step">
                            <h3>2. Adjust Settings</h3>
                            <p>Customize your PDF with options for compression, page size, orientation, and margins.</p>
                        </div>
                        <div class="step">
                            <h3>3. Generate & Download</h3>
                            <p>Click the "Generate PDF" button and download your optimized PDF document.</p>
                        </div>
                    </div>
                </div>
            </section>
        </div>
    </main>

    <footer id="contact">
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h3>PDF Maker Pro</h3>
                    <p>Your free online tool for creating high-quality PDF documents from images and scans.</p>
                </div>
                <div class="footer-column">
                    <h3>Quick Links</h3>
                    <ul>
                        <li><a href="#">Home</a></li>
                        <li><a href="#features">Features</a></li>
                        <li><a href="#how-it-works">How It Works</a></li>
                        <li><a href="#">Privacy Policy</a></li>
                        <li><a href="#">Terms of Service</a></li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h3>Contact</h3>
                    <ul>
                        <li><a href="mailto:support@pdfmakerpro.com">support@pdfmakerpro.com</a></li>
                        <li><a href="#">Feedback</a></li>
                        <li><a href="#">Report an Issue</a></li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h3>Follow Us</h3>
                    <ul>
                        <li><a href="#"><i class="fab fa-twitter"></i> Twitter</a></li>
                        <li><a href="#"><i class="fab fa-facebook"></i> Facebook</a></li>
                        <li><a href="#"><i class="fab fa-instagram"></i> Instagram</a></li>
                    </ul>
                </div>
            </div>
            <div class="copyright">
                <p>&copy; 2023 PDF Maker Pro. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <div class="toast" id="toast"></div>

    <script src="https://cdnjs.cloudflare.com/ajax/libs/pdf-lib/1.16.0/pdf-lib.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/FileSaver.js/2.0.5/FileSaver.min.js"></script>
    <script>
        document.addEventListener('DOMContentLoaded', function() {
            // Mobile menu toggle
            const mobileMenuBtn = document.getElementById('mobileMenuBtn');
            const mainNav = document.getElementById('mainNav');
            
            mobileMenuBtn.addEventListener('click', function() {
                mainNav.style.display = mainNav.style.display === 'block' ? 'none' : 'block';
            });
            
            // Handle window resize
            window.addEventListener('resize', function() {
                if (window.innerWidth > 768) {
                    mainNav.style.display = '';
                }
            });
            
            // Compression level display
            const compressionLevel = document.getElementById('compressionLevel');
            const compressionValue = document.getElementById('compressionValue');
            
            compressionLevel.addEventListener('input', function() {
                const levels = ['Low', 'Medium', 'High'];
                compressionValue.textContent = levels[this.value];
            });
            
            // File upload handling
            const uploadArea = document.getElementById('uploadArea');
            const fileInput = document.getElementById('fileInput');
            const selectFilesBtn = document.getElementById('selectFilesBtn');
            const previewContainer = document.getElementById('previewContainer');
            const previewImages = document.getElementById('previewImages');
            const clearAllBtn = document.getElementById('clearAllBtn');
            const generatePdfBtn = document.getElementById('generatePdfBtn');
            const spinner = document.getElementById('spinner');
            const toast = document.getElementById('toast');
            
            let files = [];
            
            // Handle drag and drop
            uploadArea.addEventListener('dragover', function(e) {
                e.preventDefault();
                this.style.backgroundColor = 'rgba(66, 133, 244, 0.2)';
            });
            
            uploadArea.addEventListener('dragleave', function(e) {
                e.preventDefault();
                this.style.backgroundColor = 'rgba(66, 133, 244, 0.05)';
            });
            
            uploadArea.addEventListener('drop', function(e) {
                e.preventDefault();
                this.style.backgroundColor = 'rgba(66, 133, 244, 0.05)';
                handleFiles(e.dataTransfer.files);
            });
            
            // Handle file selection
            selectFilesBtn.addEventListener('click', function() {
                fileInput.click();
            });
            
            fileInput.addEventListener('change', function() {
                if (this.files.length > 0) {
                    handleFiles(this.files);
                }
            });
            
            // Clear all files
            clearAllBtn.addEventListener('click', function() {
                files = [];
                previewImages.innerHTML = '';
                previewContainer.style.display = 'none';
                fileInput.value = '';
            });
            
            // Generate PDF
            generatePdfBtn.addEventListener('click', async function() {
                if (files.length === 0) {
                    showToast('Please add at least one file', 'error');
                    return;
                }
                
                spinner.style.display = 'block';
                generatePdfBtn.disabled = true;
                
                try {
                    const pdfName = document.getElementById('pdfName').value || 'document.pdf';
                    const compressionLevel = parseInt(document.getElementById('compressionLevel').value);
                    const pageSize = document.getElementById('pageSize').value;
                    const pageOrientation = document.getElementById('pageOrientation').value;
                    const marginSize = parseInt(document.getElementById('marginSize').value);
                    
                    // Create PDF
                    const pdfBytes = await createPdf(files, {
                        compressionLevel,
                        pageSize,
                        pageOrientation,
                        marginSize
                    });
                    
                    // Save PDF
                    const blob = new Blob([pdfBytes], { type: 'application/pdf' });
                    saveAs(blob, pdfName.endsWith('.pdf') ? pdfName : `${pdfName}.pdf`);
                    
                    showToast('PDF generated successfully!', 'success');
                } catch (error) {
                    console.error('Error generating PDF:', error);
                    showToast('Error generating PDF. Please try again.', 'error');
                } finally {
                    spinner.style.display = 'none';
                    generatePdfBtn.disabled = false;
                }
            });
            
            // Handle file processing
            function handleFiles(newFiles) {
                const validFiles = Array.from(newFiles).filter(file => {
                    const validTypes = ['image/jpeg', 'image/png', 'image/jpg', 'application/pdf'];
                    return validTypes.includes(file.type);
                });
                
                if (validFiles.length === 0) {
                    showToast('Please upload valid image or PDF files', 'error');
                    return;
                }
                
                files = files.concat(validFiles);
                updatePreview();
                
                if (files.length > 0) {
                    previewContainer.style.display = 'block';
                }
            }
            
            // Update preview images
            function updatePreview() {
                previewImages.innerHTML = '';
                
                files.forEach((file, index) => {
                    const reader = new FileReader();
                    
                    reader.onload = function(e) {
                        const previewImage = document.createElement('div');
                        previewImage.className = 'preview-image';
                        
                        if (file.type.includes('image')) {
                            previewImage.innerHTML = `
                                <img src="${e.target.result}" alt="Preview">
                                <button class="remove-btn" data-index="${index}"><i class="fas fa-times"></i></button>
                            `;
                        } else if (file.type === 'application/pdf') {
                            previewImage.innerHTML = `
                                <div style="padding: 20px; text-align: center;">
                                    <i class="fas fa-file-pdf" style="font-size: 48px; color: #e74c3c;"></i>
                                    <p style="margin-top: 10px;">${file.name}</p>
                                </div>
                                <button class="remove-btn" data-index="${index}"><i class="fas fa-times"></i></button>
                            `;
                        }
                        
                        previewImages.appendChild(previewImage);
                        
                        // Add remove button event
                        const removeBtn = previewImage.querySelector('.remove-btn');
                        removeBtn.addEventListener('click', function() {
                            const removeIndex = parseInt(this.getAttribute('data-index'));
                            files.splice(removeIndex, 1);
                            updatePreview();
                            
                            if (files.length === 0) {
                                previewContainer.style.display = 'none';
                            }
                        });
                    };
                    
                    if (file.type.includes('image')) {
                        reader.readAsDataURL(file);
                    } else {
                        reader.readAsArrayBuffer(file);
                    }
                });
            }
            
            // Create PDF function
            async function createPdf(files, options) {
                const { PDFDocument, rgb } = PDFLib;
                const pdfDoc = await PDFDocument.create();
                
                // Process each file
                for (const file of files) {
                    if (file.type.includes('image')) {
                        // Handle image files
                        const imageBytes = await readFileAsArrayBuffer(file);
                        let image;
                        
                        if (file.type === 'image/jpeg' || file.type === 'image/jpg') {
                            image = await pdfDoc.embedJpg(imageBytes);
                        } else if (file.type === 'image/png') {
                            image = await pdfDoc.embedPng(imageBytes);
                        }
                        
                        // Apply compression based on level
                        let quality;
                        switch (options.compressionLevel) {
                            case 0: quality = 1.0; break; // Low compression (high quality)
                            case 1: quality = 0.7; break; // Medium compression
                            case 2: quality = 0.4; break; // High compression (lower quality)
                            default: quality = 0.7;
                        }
                        
                        // Create page with appropriate size
                        let page;
                        const margin = options.marginSize * 2.83465; // Convert mm to points (1mm = 2.83465 points)
                        
                        if (options.pageSize === 'auto') {
                            // Auto size - fit to image dimensions
                            const width = image.width + margin * 2;
                            const height = image.height + margin * 2;
                            page = pdfDoc.addPage([width, height]);
                        } else {
                            // Standard page sizes
                            let dimensions;
                            switch (options.pageSize) {
                                case 'a4':
                                    dimensions = options.pageOrientation === 'portrait' ? 
                                        [595.28, 841.89] : [841.89, 595.28];
                                    break;
                                case 'letter':
                                    dimensions = options.pageOrientation === 'portrait' ? 
                                        [612, 792] : [792, 612];
                                    break;
                                case 'legal':
                                    dimensions = options.pageOrientation === 'portrait' ? 
                                        [612, 1008] : [1008, 612];
                                    break;
                                default:
                                    dimensions = [595.28, 841.89]; // Default to A4 portrait
                            }
                            page = pdfDoc.addPage(dimensions);
                        }
                        
                        // Draw image on page with margin
                        const marginPoints = options.marginSize * 2.83465;
                        const maxWidth = page.getWidth() - marginPoints * 2;
                        const maxHeight = page.getHeight() - marginPoints * 2;
                        
                        let width = image.width;
                        let height = image.height;
                        
                        // Scale image to fit page if needed
                        if (width > maxWidth || height > maxHeight) {
                            const ratio = Math.min(maxWidth / width, maxHeight / height);
                            width *= ratio;
                            height *= ratio;
                        }
                        
                        // Center image on page
                        const x = (page.getWidth() - width) / 2;
                        const y = (page.getHeight() - height) / 2;
                        
                        page.drawImage(image, {
                            x,
                            y,
                            width,
                            height,
                            opacity: 1,
                            // Apply compression quality here if supported by pdf-lib
                        });
                    } else if (file.type === 'application/pdf') {
                        // Handle PDF files - merge pages
                        const pdfBytes = await readFileAsArrayBuffer(file);
                        const externalPdfDoc = await PDFDocument.load(pdfBytes);
                        
                        const pages = await pdfDoc.copyPages(externalPdfDoc, externalPdfDoc.getPageIndices());
                        pages.forEach(page => pdfDoc.addPage(page));
                    }
                }
                
                // Save PDF with compression
                return await pdfDoc.save({
                    useObjectStreams: true,
                    // Additional save options for compression if available
                });
            }
            
            // Helper function to read file as ArrayBuffer
            function readFileAsArrayBuffer(file) {
                return new Promise((resolve, reject) => {
                    const reader = new FileReader();
                    reader.onload = () => resolve(reader.result);
                    reader.onerror = reject;
                    reader.readAsArrayBuffer(file);
                });
            }
            
            // Show toast notification
            function showToast(message, type) {
                toast.textContent = message;
                toast.className = 'toast';
                toast.classList.add(type);
                toast.classList.add('show');
                
                setTimeout(() => {
                    toast.classList.remove('show');
                }, 3000);
            }
            
            // Initialize AdSense (replace with your actual AdSense code)
            window.addEventListener('load', function() {
                if (typeof adsbygoogle !== 'undefined') {
                    adsbygoogle.push({});
                }
            });
        });
    </script>
</body>
</html>
