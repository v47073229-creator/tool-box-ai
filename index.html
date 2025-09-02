
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <link rel="icon" type="image/svg+xml" href="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24' fill='none' stroke='%23007BFF' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='M14.7 6.3a1 1 0 0 0 0 1.4l1.6 1.6a1 1 0 0 0 1.4 0l3.77-3.77a6 6 0 0 1-7.94 7.94l-6.91 6.91a2.12 2.12 0 0 1-3-3l6.91-6.91a6 6 0 0 1 7.94-7.94l-3.76 3.76z'/%3E%3C/svg%3E" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Toolbox.ai - Your All-in-One Toolkit</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&family=Noto+Sans:wght@400;500;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://esm.sh/react-image-crop@11.0.5/dist/ReactCrop.css">
    <style>
      body {
        font-family: 'Inter', 'Noto Sans', sans-serif;
      }
      .ReactCrop__crop-selection {
        border: 2px dashed #007BFF;
      }
    </style>
  <script type="importmap">
{
  "imports": {
    "lucide-react": "https://aistudiocdn.com/lucide-react@^0.542.0",
    "react-dom/client": "https://aistudiocdn.com/react-dom@^19.1.1/client",
    "react": "https://aistudiocdn.com/react@^19.1.1",
    "browser-image-compression": "https://esm.sh/browser-image-compression@2.0.2",
    "qrcode": "https://esm.sh/qrcode@1.5.3",
    "react-image-crop": "https://esm.sh/react-image-crop@11.0.5",
    "tesseract.js": "https://esm.sh/tesseract.js@5.1.0",
    "jsqr": "https://esm.sh/jsqr@1.4.0"
  }
}
</script>
<!-- Babel for in-browser JSX transformation -->
<script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>
</head>
  <body>
    <div id="root"></div>
    <script type="text/babel" data-type="module">
      import React, { useState, useMemo, createContext, useContext, Fragment, useEffect, useRef, useCallback } from 'react';
      import ReactDOM from 'react-dom/client';
      import { 
        Globe, Phone, Mail, X, LayoutGrid, Image as ImageIcon, Type as TypeIcon, SlidersHorizontal, 
        Calculator as CalculatorIcon, Bot, Search, Download, Lock, Unlock, RotateCcw, RotateCw, FlipHorizontal, 
        FlipVertical, RefreshCw, Clipboard, UploadCloud, Loader2, Wrench, Heart, Image, Text, ImageUp, 
        Scissors, ScanLine, FileEdit, Video, Youtube, Type, Milestone, QrCode, FileJson, ScanText, Edit, 
        GalleryThumbnails, Landmark, Trash2, Palette, Pen 
      } from 'lucide-react';
      import imageCompression from 'browser-image-compression';
      import QRCode from 'qrcode';
      import ReactCrop from 'react-image-crop';
      import { createWorker } from 'tesseract.js';
      import jsQR from 'jsqr';

      // =================================================================
      // LIB: TRANSLATIONS
      // =================================================================
      const translations = {
        // Header
        language: { en: 'Language', hi: 'भाषा' },
        english: { en: 'English', hi: 'अंग्रेजी' },
        hindi: { en: 'Hindi', hi: 'हिंदी' },
        contactUs: { en: 'Contact Us', hi: 'संपर्क करें' },

        // Sidebar
        allTools: { en: 'All Tools', hi: 'सभी उपकरण' },
        imageTools: { en: 'Image Tools', hi: 'छवि उपकरण' },
        contentTools: { en: 'Content Tools', hi: 'सामग्री उपकरण' },
        converterTools: { en: 'Converter Tools', hi: 'कनवर्टर उपकरण' },
        calculators: { en: 'Calculators', hi: 'कैलकुलेटर' },
        generators: { en: 'Generators', hi: 'जेनरेटर' },

        // ToolGrid
        searchTools: { en: 'Search for a tool...', hi: 'एक उपकरण खोजें...' },
        noToolsFound: { en: 'No tools found.', hi: 'कोई उपकरण नहीं मिला।' },

        // Footer
        howToUse: { en: 'How to Use', hi: 'कैसे उपयोग करें' },
        privacyPolicy: { en: 'Privacy Policy', hi: 'गोपनीयता नीति' },
        madeInIndia: { en: 'Made in India', hi: 'भारत में निर्मित' },
        donate: { en: 'Donate', hi: 'दान करें' },
        supportUs: { en: 'Support Us', hi: 'हमें सहयोग दें' },

        // Modals
        contactInfo: { en: 'Contact Information', hi: 'संपर्क जानकारी' },
        phone: { en: 'Phone', hi: 'फ़ोन' },
        email: { en: 'Email', hi: 'ईमेल' },
        close: { en: 'Close', hi: 'बंद करें' },
        donateTitle: { en: 'Support Our Work', hi: 'हमारे काम का समर्थन करें' },
        donateDescription: { en: 'Your contribution helps us keep these tools free for everyone. Scan the QR code or use the UPI link below.', hi: 'आपका योगदान हमें इन उपकरणों को सभी के लिए मुफ्त रखने में मदद करता है। QR कोड स्कैन करें या नीचे दिए गए UPI लिंक का उपयोग करें।' },
        scanToPay: { en: 'Scan QR to Pay', hi: 'भुगतान के लिए QR स्कैन करें' },
        payWithUPI: { en: 'Pay with UPI App', hi: 'UPI ऐप से भुगतान करें' },
        
        // UI Components
        uploadFile: { en: 'Upload File', hi: 'फ़ाइल अपलोड करें' },
        dragDrop: { en: 'or drag and drop', hi: 'या खींच कर छोड़ें' },
        download: { en: 'Download', hi: 'डाउनलोड' },

        // Image Compressor
        compressing: { en: 'Compressing...', hi: 'संपीड़ित हो रहा है...' },
        compress: { en: 'Compress', hi: 'संपीड़ित करें' },
        quality: { en: 'Quality', hi: 'गुणवत्ता' },
        originalSize: { en: 'Original Size', hi: 'मूल आकार' },
        compressedSize: { en: 'Compressed Size', hi: 'संपीड़ित आकार' },
        sizeReduction: { en: 'Size Reduction', hi: 'आकार में कमी' },

        // Text to QR Code
        enterText: { en: 'Enter text or URL', hi: 'टेक्स्ट या यूआरएल दर्ज करें' },

        // JSON Formatter
        formatJson: { en: 'Format JSON', hi: 'JSON प्रारूपित करें' },
        pasteJson: { en: 'Paste your JSON here...', hi: 'अपना JSON यहां पेस्ट करें...' },
        invalidJson: { en: 'Invalid JSON', hi: 'अमान्य JSON' },
        
        // Image Resizer
        width: { en: 'Width', hi: 'चौड़ाई' },
        height: { en: 'Height', hi: 'ऊंचाई' },
        lockAspectRatio: { en: 'Lock aspect ratio', hi: 'पहलू अनुपात लॉक करें' },
        resize: { en: 'Resize', hi: 'आकार बदलें' },
        originalDimensions: { en: 'Original Dimensions', hi: 'मूल आयाम' },
        newDimensions: { en: 'New Dimensions', hi: 'नए आयाम' },

        // Passport Photo Maker
        cropInstruction: { en: 'Drag the selection to crop your photo to a 3:4 aspect ratio.', hi: '3:4 पहलू अनुपात में अपनी तस्वीर काटने के लिए चयन को खींचें।' },
        cropAndDownload: { en: 'Crop & Download', hi: 'काटें और डाउनलोड करें' },

        // Image Editor
        rotateLeft: { en: 'Rotate Left', hi: 'बाएं घुमाएं' },
        rotateRight: { en: 'Rotate Right', hi: 'दाएं घुमाएं' },
        flipHorizontal: { en: 'Flip Horizontal', hi: 'क्षैतिज रूप से पलटें' },
        flipVertical: { en: 'Flip Vertical', hi: 'लंबवत रूप से पलटें' },
        grayscale: { en: 'Grayscale', hi: 'ग्रेस्केल' },
        sepia: { en: 'Sepia', hi: 'सेपिया' },
        invert: { en: 'Invert', hi: 'उलटा' },
        reset: { en: 'Reset', hi: 'रीसेट' },
        
        // YouTube Title Generator
        enterKeywords: { en: 'Enter keywords (e.g., easy cookies, home recipe)', hi: 'कीवर्ड दर्ज करें (जैसे, आसान कुकीज़, घरेलू रेसिपी)' },
        generateTitles: { en: 'Generate Titles', hi: 'शीर्षक उत्पन्न करें' },
        generatedTitles: { en: 'Generated Titles', hi: 'उत्पन्न शीर्षक' },

        // Image to Text (OCR)
        recognizeText: { en: 'Recognize Text', hi: 'पाठ पहचानें' },
        recognizing: { en: 'Recognizing...', hi: 'पहचान हो रही है...' },
        progress: { en: 'Progress', hi: 'प्रगति' },
        selectLanguage: { en: 'Select Language for OCR', hi: 'ओसीआर के लिए भाषा चुनें' },
        eng: { en: 'English', hi: 'अंग्रेजी' },
        hin: { en: 'Hindi', hi: 'हिंदी' },
        extractedText: { en: 'Extracted Text', hi: 'निकाला गया पाठ' },

        // Screenshot Editor
        brushColor: { en: 'Brush Color', hi: 'ब्रश का रंग' },
        brushSize: { en: 'Brush Size', hi: 'ब्रश का आकार' },
        drawOnImage: { en: 'Draw on your image', hi: 'अपनी छवि पर ड्रा करें' },
        clearDrawing: { en: 'Clear Drawing', hi: 'ड्राइंग साफ़ करें' },

        // YouTube Thumbnail Generator
        controls: { en: 'Controls', hi: 'नियंत्रण' },
        titleText: { en: 'Title Text', hi: 'शीर्षक पाठ' },
        backgroundColor: { en: 'Background Color', hi: 'पृष्ठभूमि का रंग' },
        textColor: { en: 'Text Color', hi: 'पाठ का रंग' },
        fontSize: { en: 'Font Size', hi: 'फ़ॉन्ट का आकार' },
        uploadBackground: { en: 'Upload Background Image', hi: 'पृष्ठभूमि छवि अपलोड करें' },
        thumbnailPreview: { en: 'Thumbnail Preview', hi: 'थंबनेल पूर्वावलोकन' },

        // Image to QR Code
        scanQrCode: { en: 'Scan QR Code', hi: 'क्यूआर कोड स्कैन करें' },
        noQrCodeFound: { en: 'No QR code found in the image.', hi: 'छवि में कोई क्यूआर कोड नहीं मिला।' },
        decodedText: { en: 'Decoded Text', hi: 'डिकोड किया गया पाठ' },

        // Finance Calculator
        emiCalculator: { en: 'EMI Calculator', hi: 'ईएमआई कैलकुलेटर' },
        simpleInterest: { en: 'Simple Interest', hi: 'साधारण ब्याज' },
        compoundInterest: { en: 'Compound Interest', hi: 'चक्रवृद्धि ब्याज' },
        principalAmount: { en: 'Principal Amount', hi: 'मूल राशि' },
        annualInterestRate: { en: 'Annual Interest Rate (%)', hi: 'वार्षिक ब्याज दर (%)' },
        loanTenureYears: { en: 'Loan Tenure (Years)', hi: 'ऋण अवधि (वर्ष)' },
        monthlyEMI: { en: 'Monthly EMI', hi: 'मासिक ईएमआई' },
        calculate: { en: 'Calculate', hi: 'गणना करें' },
        totalInterest: { en: 'Total Interest', hi: 'कुल ब्याज' },
        totalAmount: { en: 'Total Amount', hi: 'कुल राशि' },
        timePeriodYears: { en: 'Time Period (Years)', hi: 'समय अवधि (वर्ष)' },
        compoundingFrequency: { en: 'Compounding Frequency', hi: 'चक्रवृद्धि आवृत्ति' },
        annually: { en: 'Annually', hi: 'वार्षिक' },
        semiAnnually: { en: 'Semi-Annually', hi: 'अर्ध-वार्षिक' },
        quarterly: { en: 'Quarterly', hi: 'त्रैमासिक' },
        monthly: { en: 'Monthly', hi: 'मासिक' },
      };

      // =================================================================
      // CONTEXT: LANGUAGE
      // =================================================================
      const LanguageContext = createContext(undefined);

      const LanguageProvider = ({ children }) => {
        const [language, setLanguage] = useState('en');
        return (
          <LanguageContext.Provider value={{ language, setLanguage }}>
            {children}
          </LanguageContext.Provider>
        );
      };

      const useLanguage = () => {
        const context = useContext(LanguageContext);
        if (!context) {
          throw new Error('useLanguage must be used within a LanguageProvider');
        }
        return context;
      };

      // =================================================================
      // HOOK: USE TRANSLATION
      // =================================================================
      const useTranslation = () => {
        const { language } = useLanguage();

        const t = (key) => {
          return translations[key][language];
        };
        
        const getLocalized = (localizedString) => {
          return localizedString[language];
        }

        return { t, getLocalized, language };
      };
      
      // =================================================================
      // UI COMPONENT: Button
      // =================================================================
      const Button = ({ children, className, isLoading = false, icon, ...props }) => {
        return (
          <button
            className={`inline-flex items-center justify-center px-6 py-3 font-semibold text-white bg-blue-500 rounded-lg hover:bg-blue-600 focus:outline-none focus:ring-2 focus:ring-blue-500 focus:ring-opacity-50 transition-all duration-300 transform hover:scale-105 disabled:bg-slate-400 disabled:cursor-not-allowed disabled:scale-100 ${className}`}
            disabled={isLoading}
            {...props}
          >
            {isLoading ? (
              <Loader2 className="w-5 h-5 mr-2 animate-spin" />
            ) : (
              icon && <span className="mr-2">{icon}</span>
            )}
            {children}
          </button>
        );
      };

      // =================================================================
      // UI COMPONENT: FileDropzone
      // =================================================================
      const FileDropzone = ({ onFileAccepted, acceptedFileTypes }) => {
        const [isDragging, setIsDragging] = useState(false);
        const { t } = useTranslation();

        const handleDragEnter = (e) => {
          e.preventDefault();
          e.stopPropagation();
          setIsDragging(true);
        };

        const handleDragLeave = (e) => {
          e.preventDefault();
          e.stopPropagation();
          setIsDragging(false);
        };

        const handleDragOver = (e) => {
          e.preventDefault();
          e.stopPropagation();
        };

        const handleDrop = useCallback((e) => {
          e.preventDefault();
          e.stopPropagation();
          setIsDragging(false);
          if (e.dataTransfer.files && e.dataTransfer.files.length > 0) {
            onFileAccepted(e.dataTransfer.files[0]);
            e.dataTransfer.clearData();
          }
        }, [onFileAccepted]);
        
        const handleFileChange = (e) => {
          if (e.target.files && e.target.files.length > 0) {
            onFileAccepted(e.target.files[0]);
          }
        };

        return (
          <div
            className={`relative flex flex-col items-center justify-center w-full p-8 border-2 border-dashed rounded-xl transition-colors duration-300
              ${isDragging ? 'border-blue-500 bg-blue-50' : 'border-slate-300 bg-slate-50'}`}
            onDragEnter={handleDragEnter}
            onDragLeave={handleDragLeave}
            onDragOver={handleDragOver}
            onDrop={handleDrop}
          >
            <UploadCloud className="w-12 h-12 text-slate-400 mb-4" />
            <label htmlFor="file-upload" className="font-semibold text-blue-600 cursor-pointer hover:underline">
              {t('uploadFile')}
              <input id="file-upload" name="file-upload" type="file" className="sr-only" onChange={handleFileChange} accept={acceptedFileTypes} />
            </label>
            <p className="mt-1 text-sm text-slate-500">{t('dragDrop')}</p>
          </div>
        );
      };
      
      // =================================================================
      // UI COMPONENT: Slider
      // =================================================================
      const Slider = ({ label, value, ...props }) => {
        return (
          <div className="w-full">
            <label className="flex justify-between items-center text-sm font-medium text-slate-700 mb-2">
              <span>{label}</span>
              <span className="font-bold text-blue-600">{value}</span>
            </label>
            <input
              type="range"
              className="w-full h-2 bg-slate-200 rounded-lg appearance-none cursor-pointer"
              style={{
                  background: `linear-gradient(to right, #3B82F6 0%, #3B82F6 ${value}%, #E2E8F0 ${value}%, #E2E8F0 100%)`
              }}
              {...props}
            />
          </div>
        );
      };
      
      // =================================================================
      // TOOL: Placeholder
      // =================================================================
      const PlaceholderTool = () => {
        return (
          <div className="flex flex-col items-center justify-center text-center p-8 bg-slate-50 rounded-lg border-2 border-dashed border-slate-300" aria-live="polite">
            <Wrench className="w-16 h-16 text-slate-400 mb-4" aria-hidden="true" />
            <h3 className="text-xl font-semibold text-slate-700 mb-2">
              Tool Under Construction
            </h3>
            <p className="text-slate-500 max-w-md">
              We are working hard to bring this feature to you soon. All tools on this platform work directly in your browser without needing any server-side processing or API keys.
            </p>
          </div>
        );
      };

      // =================================================================
      // TOOL: Image Compressor
      // =================================================================
      const ImageCompressor = () => {
        const [originalFile, setOriginalFile] = useState(null);
        const [originalUrl, setOriginalUrl] = useState('');
        const [compressedUrl, setCompressedUrl] = useState('');
        const [compressedFile, setCompressedFile] = useState(null);
        const [quality, setQuality] = useState(80);
        const [isLoading, setIsLoading] = useState(false);
        const { t } = useTranslation();

        const handleFileAccepted = (file) => {
          setOriginalFile(file);
          setOriginalUrl(URL.createObjectURL(file));
          setCompressedUrl('');
          setCompressedFile(null);
        };

        const handleCompress = async () => {
          if (!originalFile) return;
          setIsLoading(true);
          try {
            const options = {
              maxSizeMB: 2,
              maxWidthOrHeight: 1920,
              useWebWorker: true,
              initialQuality: quality / 100,
            };
            const compressed = await imageCompression(originalFile, options);
            setCompressedFile(compressed);
            setCompressedUrl(URL.createObjectURL(compressed));
          } catch (error) {
            console.error(error);
          } finally {
            setIsLoading(false);
          }
        };

        const formatBytes = (bytes, decimals = 2) => {
          if (bytes === 0) return '0 Bytes';
          const k = 1024;
          const dm = decimals < 0 ? 0 : decimals;
          const sizes = ['Bytes', 'KB', 'MB', 'GB'];
          const i = Math.floor(Math.log(bytes) / Math.log(k));
          return parseFloat((bytes / Math.pow(k, i)).toFixed(dm)) + ' ' + sizes[i];
        };

        return (
          <div className="space-y-6">
            {!originalFile && (
              <FileDropzone onFileAccepted={handleFileAccepted} acceptedFileTypes="image/jpeg, image/png, image/webp" />
            )}

            {originalFile && (
              <div className="grid grid-cols-1 md:grid-cols-2 gap-6 items-center">
                  <div className="text-center">
                       <h3 className="font-semibold text-lg mb-2">{t('originalSize')}: {formatBytes(originalFile.size)}</h3>
                       <img src={originalUrl} alt="Original" className="max-w-full h-auto rounded-lg shadow-md mx-auto" style={{ maxHeight: '300px' }} />
                  </div>
                   <div className="text-center">
                      {compressedFile ? (
                          <>
                              <h3 className="font-semibold text-lg mb-2">{t('compressedSize')}: {formatBytes(compressedFile.size)}</h3>
                              <img src={compressedUrl} alt="Compressed" className="max-w-full h-auto rounded-lg shadow-md mx-auto" style={{ maxHeight: '300px' }} />
                          </>
                      ) : (
                          <div className="flex items-center justify-center h-full text-slate-500">{isLoading ? t('compressing') : ''}</div>
                      )}
                  </div>
              </div>
            )}

            {originalFile && (
              <div className="bg-slate-50 p-6 rounded-lg space-y-4">
                <Slider label={t('quality')} value={quality} min="1" max="100" onChange={(e) => setQuality(Number(e.target.value))} />
                <div className="flex flex-col sm:flex-row gap-4">
                  <Button onClick={handleCompress} isLoading={isLoading} className="flex-1">
                    {isLoading ? t('compressing') : t('compress')}
                  </Button>
                  {compressedFile && (
                    <a href={compressedUrl} download={compressedFile.name}>
                      <Button className="w-full" icon={<Download />}>
                        {t('download')}
                      </Button>
                    </a>
                  )}
                </div>
                  {originalFile && compressedFile && (
                      <p className="text-center text-green-600 font-semibold">{t('sizeReduction')}: {(((originalFile.size - compressedFile.size) / originalFile.size) * 100).toFixed(1)}%</p>
                  )}
              </div>
            )}
          </div>
        );
      };
      
      // =================================================================
      // TOOL: TextToQRCode
      // =================================================================
      const TextToQRCode = () => {
        const [text, setText] = useState('');
        const [qrCodeUrl, setQrCodeUrl] = useState('');
        const { t } = useTranslation();

        useEffect(() => {
          if (text.trim() === '') {
              setQrCodeUrl('');
              return;
          }
          
          const generateQRCode = async () => {
              try {
                  const url = await QRCode.toDataURL(text, { errorCorrectionLevel: 'H', width: 256 });
                  setQrCodeUrl(url);
              } catch (err) {
                  console.error(err);
              }
          };

          const timeoutId = setTimeout(generateQRCode, 300); // Debounce
          return () => clearTimeout(timeoutId);

        }, [text]);

        return (
          <div className="flex flex-col items-center space-y-6">
            <textarea
              value={text}
              onChange={(e) => setText(e.target.value)}
              placeholder={t('enterText')}
              className="w-full p-4 border-2 border-slate-200 rounded-lg focus:outline-none focus:border-blue-500 transition-colors"
              rows={4}
            />

            {qrCodeUrl && (
              <div className="p-4 bg-white rounded-lg shadow-md border">
                <img src={qrCodeUrl} alt="Generated QR Code" width="256" height="256" />
              </div>
            )}
            
            {qrCodeUrl && (
               <a href={qrCodeUrl} download="qrcode.png">
                  <Button icon={<Download />}>
                      {t('download')}
                  </Button>
              </a>
            )}
          </div>
        );
      };
      
      // =================================================================
      // TOOL: JSON Formatter
      // =================================================================
      const JSONFormatter = () => {
        const [inputJson, setInputJson] = useState('');
        const [formattedJson, setFormattedJson] = useState('');
        const [error, setError] = useState('');
        const { t } = useTranslation();

        const handleFormat = () => {
          try {
            if (inputJson.trim() === '') {
              setError('');
              setFormattedJson('');
              return;
            }
            const parsed = JSON.parse(inputJson);
            const formatted = JSON.stringify(parsed, null, 2);
            setFormattedJson(formatted);
            setError('');
          } catch (e) {
            setError(t('invalidJson'));
            setFormattedJson('');
          }
        };

        return (
          <div className="space-y-4">
            <textarea
              value={inputJson}
              onChange={(e) => setInputJson(e.target.value)}
              placeholder={t('pasteJson')}
              className={`w-full p-4 border-2 rounded-lg focus:outline-none transition-colors font-mono ${error ? 'border-red-500' : 'border-slate-200 focus:border-blue-500'}`}
              rows={8}
            />
            
            {error && <p className="text-red-500 text-sm">{error}</p>}
            
            <Button onClick={handleFormat}>{t('formatJson')}</Button>

            {formattedJson && (
              <pre className="w-full p-4 bg-slate-100 rounded-lg text-sm overflow-x-auto">
                <code>{formattedJson}</code>
              </pre>
            )}
          </div>
        );
      };

      // =================================================================
      // TOOL: Calculator
      // =================================================================
      const AppCalculator = () => {
        const [display, setDisplay] = useState('0');
        const [expression, setExpression] = useState('');

        const handleButtonClick = (value) => {
          if (value === 'C') {
            setDisplay('0');
            setExpression('');
          } else if (value === '=') {
            try {
              const result = new Function('return ' + expression)();
              setDisplay(String(result));
              setExpression(String(result));
            } catch (e) {
              setDisplay('Error');
              setExpression('');
            }
          } else if (value === '←') {
              if(expression.length > 1) {
                  const newExpression = expression.slice(0, -1);
                  setExpression(newExpression);
                  setDisplay(newExpression);
              } else {
                  setExpression('');
                  setDisplay('0');
              }
          } else {
            const newExpression = expression === '' || expression === '0' ? value : expression + value;
            setExpression(newExpression);
            setDisplay(newExpression);
          }
        };

        const buttons = [
          'C', '(', ')', '/',
          '7', '8', '9', '*',
          '4', '5', '6', '-',
          '1', '2', '3', '+',
          '0', '.', '←', '=',
        ];

        const getButtonClass = (btn) => {
          if (['/', '*', '-', '+', '='].includes(btn)) {
            return 'bg-blue-500 hover:bg-blue-600 text-white';
          }
          if (['C', '←'].includes(btn)) {
            return 'bg-slate-200 hover:bg-slate-300';
          }
          return 'bg-white hover:bg-slate-100';
        };

        return (
          <div className="max-w-xs mx-auto bg-slate-50 border-4 border-slate-200 rounded-2xl shadow-lg p-4 space-y-4">
            <div className="bg-white text-right text-4xl font-sans font-semibold p-4 rounded-lg break-all shadow-inner">
              {display}
            </div>
            <div className="grid grid-cols-4 gap-2">
              {buttons.map((btn) => (
                <button
                  key={btn}
                  onClick={() => handleButtonClick(btn)}
                  className={`text-2xl font-bold p-4 rounded-lg transition-all transform hover:scale-105 ${getButtonClass(btn)}`}
                >
                  {btn}
                </button>
              ))}
            </div>
          </div>
        );
      };
      
      // =================================================================
      // TOOL: Image Resizer
      // =================================================================
      const ImageResizer = () => {
          const [originalFile, setOriginalFile] = useState(null);
          const [originalUrl, setOriginalUrl] = useState('');
          const [originalDimensions, setOriginalDimensions] = useState({ width: 0, height: 0 });
          const [newWidth, setNewWidth] = useState('');
          const [newHeight, setNewHeight] = useState('');
          const [lockAspectRatio, setLockAspectRatio] = useState(true);
          const [resizedUrl, setResizedUrl] = useState('');
          const { t } = useTranslation();
          const imageRef = useRef(null);

          const handleFileAccepted = (file) => {
              setOriginalFile(file);
              const url = URL.createObjectURL(file);
              setOriginalUrl(url);
              setResizedUrl('');

              const img = new window.Image();
              img.onload = () => {
                  setOriginalDimensions({ width: img.width, height: img.height });
                  setNewWidth(String(img.width));
                  setNewHeight(String(img.height));
              };
              img.src = url;
          };

          const handleWidthChange = (e) => {
              const width = e.target.value;
              setNewWidth(width);
              if (lockAspectRatio && originalDimensions.width > 0) {
                  const aspectRatio = originalDimensions.height / originalDimensions.width;
                  setNewHeight(String(Math.round(Number(width) * aspectRatio)));
              }
          };

          const handleHeightChange = (e) => {
              const height = e.target.value;
              setNewHeight(height);
              if (lockAspectRatio && originalDimensions.height > 0) {
                  const aspectRatio = originalDimensions.width / originalDimensions.height;
                  setNewWidth(String(Math.round(Number(height) * aspectRatio)));
              }
          };

          const handleResize = () => {
              if (!originalUrl) return;
              const img = imageRef.current;
              if (!img) return;

              const canvas = document.createElement('canvas');
              canvas.width = Number(newWidth);
              canvas.height = Number(newHeight);
              const ctx = canvas.getContext('2d');
              if (!ctx) return;
              
              ctx.drawImage(img, 0, 0, Number(newWidth), Number(newHeight));
              setResizedUrl(canvas.toDataURL(originalFile?.type));
          };

          return (
              <div className="space-y-6">
                  {!originalFile && (
                      <FileDropzone onFileAccepted={handleFileAccepted} acceptedFileTypes="image/jpeg, image/png, image/webp" />
                  )}
                  {originalFile && (
                      <div>
                           <img src={originalUrl} ref={imageRef} alt="Original Preview" className="max-w-full h-auto rounded-lg shadow-md mx-auto hidden" />
                           <div className="bg-slate-50 p-6 rounded-lg space-y-4">
                              <div className="text-center font-medium text-slate-600">{t('originalDimensions')}: {originalDimensions.width} x {originalDimensions.height}</div>
                              <div className="flex items-center gap-4">
                                  <div className="flex-1">
                                      <label className="block text-sm font-medium text-slate-700">{t('width')}</label>
                                      <input type="number" value={newWidth} onChange={handleWidthChange} className="w-full p-2 border-2 border-slate-200 rounded-lg"/>
                                  </div>
                                  <button onClick={() => setLockAspectRatio(!lockAspectRatio)} className="mt-6 p-2">
                                      {lockAspectRatio ? <Lock className="text-blue-500" /> : <Unlock className="text-slate-500" />}
                                  </button>
                                  <div className="flex-1">
                                      <label className="block text-sm font-medium text-slate-700">{t('height')}</label>
                                      <input type="number" value={newHeight} onChange={handleHeightChange} className="w-full p-2 border-2 border-slate-200 rounded-lg"/>
                                  </div>
                              </div>
                              <Button onClick={handleResize} className="w-full">{t('resize')}</Button>
                           </div>
                      </div>
                  )}
                  {resizedUrl && (
                      <div className="text-center space-y-4">
                          <h3 className="font-semibold text-lg">{t('newDimensions')}: {newWidth} x {newHeight}</h3>
                          <img src={resizedUrl} alt="Resized Preview" className="max-w-full h-auto rounded-lg shadow-md mx-auto" style={{ maxHeight: '300px' }} />
                          <a href={resizedUrl} download={`resized-${originalFile?.name}`}>
                              <Button icon={<Download />}>{t('download')}</Button>
                          </a>
                      </div>
                  )}
              </div>
          );
      };
      
      // =================================================================
      // TOOL: Passport Photo Maker
      // =================================================================
      const PassportPhotoMaker = () => {
          const [imgSrc, setImgSrc] = useState('');
          const [crop, setCrop] = useState();
          const [completedCrop, setCompletedCrop] = useState();
          const imgRef = useRef(null);
          const { t } = useTranslation();

          const handleFileAccepted = (file) => {
              setCrop(undefined); 
              setImgSrc(URL.createObjectURL(file));
          };

          const handleDownload = () => {
              if (!completedCrop || !imgRef.current) {
                  return;
              }

              const image = imgRef.current;
              const canvas = document.createElement('canvas');
              const scaleX = image.naturalWidth / image.width;
              const scaleY = image.naturalHeight / image.height;
              
              canvas.width = completedCrop.width * scaleX;
              canvas.height = completedCrop.height * scaleY;
              
              const ctx = canvas.getContext('2d');
              if (!ctx) {
                  return;
              }

              ctx.drawImage(
                  image,
                  completedCrop.x * scaleX,
                  completedCrop.y * scaleY,
                  completedCrop.width * scaleX,
                  completedCrop.height * scaleY,
                  0,
                  0,
                  canvas.width,
                  canvas.height
              );
              
              const dataUrl = canvas.toDataURL('image/jpeg');
              const link = document.createElement('a');
              link.download = 'passport-photo.jpg';
              link.href = dataUrl;
              link.click();
          };

          return (
              <div className="space-y-6">
                  {!imgSrc && (
                      <FileDropzone onFileAccepted={handleFileAccepted} acceptedFileTypes="image/jpeg, image/png" />
                  )}
                  {imgSrc && (
                      <div className="flex flex-col items-center space-y-4">
                          <p className="text-center text-slate-600">{t('cropInstruction')}</p>
                          <div className="max-w-full overflow-hidden rounded-lg border">
                              <ReactCrop
                                  crop={crop}
                                  onChange={c => setCrop(c)}
                                  onComplete={c => setCompletedCrop(c)}
                                  aspect={3 / 4}
                                  minWidth={100}
                              >
                                  <img ref={imgRef} src={imgSrc} alt="Crop preview" style={{ maxHeight: '50vh' }}/>
                              </ReactCrop>
                          </div>
                           <Button onClick={handleDownload} disabled={!completedCrop?.width} icon={<Download />}>
                              {t('cropAndDownload')}
                          </Button>
                      </div>
                  )}
              </div>
          );
      };

      // =================================================================
      // TOOL: Image Editor
      // =================================================================
      const ImageEditor = () => {
          const [imgSrc, setImgSrc] = useState('');
          const [rotation, setRotation] = useState(0);
          const [scaleX, setScaleX] = useState(1);
          const [scaleY, setScaleY] = useState(1);
          const [filters, setFilters] = useState({ grayscale: 0, sepia: 0, invert: 0 });
          const canvasRef = useRef(null);
          const imageRef = useRef(null);
          const { t } = useTranslation();

          const applyTransformations = () => {
            if (!imgSrc || !canvasRef.current || !imageRef.current) return;
            const canvas = canvasRef.current;
            const image = imageRef.current;
            const ctx = canvas.getContext('2d');
            if (!ctx) return;
            
            const w = image.naturalWidth;
            const h = image.naturalHeight;
            
            const rad = rotation * Math.PI / 180;
            const absCos = Math.abs(Math.cos(rad));
            const absSin = Math.abs(Math.sin(rad));
            
            canvas.width = w * absCos + h * absSin;
            canvas.height = h * absCos + w * absSin;

            ctx.filter = `grayscale(${filters.grayscale}%) sepia(${filters.sepia}%) invert(${filters.invert}%)`;

            ctx.translate(canvas.width / 2, canvas.height / 2);
            ctx.rotate(rad);
            ctx.scale(scaleX, scaleY);
            ctx.drawImage(image, -w / 2, -h / 2);
          };

          useEffect(() => {
              if (imgSrc && imageRef.current) {
                  const image = imageRef.current;
                  if (image.complete) {
                      applyTransformations();
                  } else {
                      image.onload = applyTransformations;
                  }
              }
          }, [imgSrc, rotation, scaleX, scaleY, filters]);

          const handleFileAccepted = (file) => {
              setImgSrc(URL.createObjectURL(file));
              reset();
          };

          const handleFilter = (filterName) => {
              setFilters(prev => ({ ...prev, [filterName]: prev[filterName] > 0 ? 0 : 100 }));
          };
          
          const reset = () => {
              setRotation(0);
              setScaleX(1);
              setScaleY(1);
              setFilters({ grayscale: 0, sepia: 0, invert: 0 });
          }

          const handleDownload = () => {
              if (!canvasRef.current) return;
              const link = document.createElement('a');
              link.download = 'edited-image.png';
              link.href = canvasRef.current.toDataURL();
              link.click();
          };

          const controlButtons = [
              { icon: <RotateCcw />, label: t('rotateLeft'), action: () => setRotation(r => r - 90) },
              { icon: <RotateCw />, label: t('rotateRight'), action: () => setRotation(r => r + 90) },
              { icon: <FlipHorizontal />, label: t('flipHorizontal'), action: () => setScaleX(s => s * -1) },
              { icon: <FlipVertical />, label: t('flipVertical'), action: () => setScaleY(s => s * -1) },
          ];
          
          const filterButtons = [
              { label: t('grayscale'), key: 'grayscale' },
              { label: t('sepia'), key: 'sepia' },
              { label: t('invert'), key: 'invert' },
          ];

          return (
              <div className="space-y-6">
                  {!imgSrc && <FileDropzone onFileAccepted={handleFileAccepted} acceptedFileTypes="image/jpeg, image/png" />}
                  {imgSrc && (
                      <div className="flex flex-col items-center space-y-4">
                          <img ref={imageRef} src={imgSrc} className="hidden" />
                          <canvas ref={canvasRef} className="max-w-full h-auto rounded-lg shadow-md" style={{maxHeight: '40vh'}}/>
                          
                          <div className="bg-slate-50 p-4 rounded-lg w-full max-w-lg space-y-4">
                              <div className="grid grid-cols-2 md:grid-cols-4 gap-2">
                                 {controlButtons.map(btn => (
                                     <button key={btn.label} onClick={btn.action} className="flex flex-col items-center p-2 rounded-lg hover:bg-slate-200 transition-colors">
                                         {btn.icon}
                                         <span className="text-xs mt-1">{btn.label}</span>
                                     </button>
                                 ))}
                              </div>
                              <div className="grid grid-cols-3 gap-2">
                                  {filterButtons.map(btn => (
                                     <button key={btn.label} onClick={() => handleFilter(btn.key)} className={`p-2 rounded-lg transition-colors ${filters[btn.key] > 0 ? 'bg-blue-500 text-white' : 'bg-slate-200 hover:bg-slate-300'}`}>{btn.label}</button>
                                  ))}
                              </div>
                              <div className="flex gap-2">
                                 <Button onClick={reset} className="flex-1 bg-slate-600 hover:bg-slate-700" icon={<RefreshCw/>}>{t('reset')}</Button>
                                 <Button onClick={handleDownload} className="flex-1" icon={<Download />}>{t('download')}</Button>
                              </div>
                          </div>
                      </div>
                  )}
              </div>
          );
      };

      // =================================================================
      // TOOL: YouTube Title Generator
      // =================================================================
      const YouTubeTitleGenerator = () => {
          const [keywords, setKeywords] = useState('');
          const [titles, setTitles] = useState([]);
          const [copiedIndex, setCopiedIndex] = useState(null);
          const { t } = useTranslation();

          const templates = [
              "How to [KW] - The Ultimate Guide",
              "[KW]: A Beginner's Tutorial",
              "The Top 5 Mistakes to Avoid When [KW]",
              "Mastering [KW] in Just 10 Minutes",
              "The Secret to Perfect [KW] Revealed",
              "[KW] vs [COMPETITOR]: Which is Better?",
              "My Honest Review of [KW]",
              "Why Everyone is Talking About [KW]",
              "The Complete [KW] Walkthrough for 2024",
              "DIY [KW] on a Budget"
          ];

          const generateTitles = () => {
              if (!keywords.trim()) return;
              const kw = keywords.trim();
              const generated = templates.map(template => 
                  template.replace(/\[KW\]/g, kw).replace(/\[COMPETITOR\]/g, 'Others')
              );
              setTitles(generated);
          };
          
          const handleCopy = (text, index) => {
              navigator.clipboard.writeText(text);
              setCopiedIndex(index);
              setTimeout(() => setCopiedIndex(null), 2000);
          };

          return (
              <div className="space-y-6">
                  <div className="space-y-2">
                      <label htmlFor="keywords" className="font-semibold text-slate-700">{t('enterKeywords')}</label>
                      <input
                          id="keywords"
                          type="text"
                          value={keywords}
                          onChange={(e) => setKeywords(e.target.value)}
                          placeholder={t('enterKeywords')}
                          className="w-full p-3 border-2 border-slate-200 rounded-lg focus:outline-none focus:border-blue-500 transition-colors"
                      />
                  </div>
                  <Button onClick={generateTitles} className="w-full sm:w-auto">{t('generateTitles')}</Button>

                  {titles.length > 0 && (
                      <div className="space-y-3">
                          <h3 className="font-bold text-xl">{t('generatedTitles')}</h3>
                          <ul className="space-y-2">
                              {titles.map((title, index) => (
                                  <li key={index} className="flex items-center justify-between p-3 bg-slate-50 rounded-lg">
                                      <span className="flex-1 mr-4">{title}</span>
                                      <button onClick={() => handleCopy(title, index)} className="relative p-2 text-slate-500 hover:text-blue-600 hover:bg-slate-200 rounded-full transition-colors">
                                          <Clipboard size={18} />
                                          {copiedIndex === index && <span className="absolute bottom-full left-1/2 -translate-x-1/2 mb-2 text-xs bg-slate-800 text-white p-1 rounded">Copied!</span>}
                                      </button>
                                  </li>
                              ))}
                          </ul>
                      </div>
                  )}
              </div>
          );
      };
      
      // =================================================================
      // TOOL: Image to Text (OCR)
      // =================================================================
      const ImageToText = () => {
          const [imageFile, setImageFile] = useState(null);
          const [imageUrl, setImageUrl] = useState('');
          const [ocrResult, setOcrResult] = useState('');
          const [progress, setProgress] = useState(0);
          const [isLoading, setIsLoading] = useState(false);
          const [ocrLanguage, setOcrLanguage] = useState('eng');
          const { t } = useTranslation();

          const handleFileAccepted = (file) => {
              setImageFile(file);
              setImageUrl(URL.createObjectURL(file));
              setOcrResult('');
              setProgress(0);
          };

          const handleRecognize = async () => {
              if (!imageFile) return;

              setIsLoading(true);
              setProgress(0);
              const worker = await createWorker(ocrLanguage, 1, {
                  logger: m => {
                      if (m.status === 'recognizing text') {
                          setProgress(Math.round(m.progress * 100));
                      }
                  },
              });
              
              const { data: { text } } = await worker.recognize(imageFile);
              setOcrResult(text);
              setIsLoading(false);
              await worker.terminate();
          };
          
          const handleCopy = () => {
              navigator.clipboard.writeText(ocrResult);
          };

          return (
              <div className="space-y-6">
                  {!imageFile && (
                      <FileDropzone onFileAccepted={handleFileAccepted} acceptedFileTypes="image/jpeg, image/png, image/webp" />
                  )}

                  {imageFile && (
                      <div className="space-y-4">
                          <img src={imageUrl} alt="Uploaded for OCR" className="max-w-full h-auto rounded-lg shadow-md mx-auto" style={{ maxHeight: '300px' }} />
                          <div className="bg-slate-50 p-4 rounded-lg space-y-4">
                              <div>
                                  <label className="block text-sm font-medium text-slate-700 mb-2">{t('selectLanguage')}</label>
                                  <select
                                      value={ocrLanguage}
                                      onChange={(e) => setOcrLanguage(e.target.value)}
                                      className="w-full p-2 border-2 border-slate-200 rounded-lg"
                                      disabled={isLoading}
                                  >
                                      <option value="eng">{t('eng')}</option>
                                      <option value="hin">{t('hin')}</option>
                                  </select>
                              </div>
                              <Button onClick={handleRecognize} isLoading={isLoading} className="w-full">
                                  {isLoading ? `${t('recognizing')}...` : t('recognizeText')}
                              </Button>
                          </div>
                      </div>
                  )}
                  
                  {isLoading && (
                       <div className="w-full">
                          <div className="flex justify-between mb-1">
                              <span className="text-base font-medium text-blue-700">{t('progress')}</span>
                              <span className="text-sm font-medium text-blue-700">{progress}%</span>
                          </div>
                          <div className="w-full bg-slate-200 rounded-full h-2.5">
                              <div className="bg-blue-600 h-2.5 rounded-full" style={{ width: `${progress}%` }}></div>
                          </div>
                      </div>
                  )}

                  {ocrResult && (
                      <div className="space-y-2">
                          <div className="flex justify-between items-center">
                              <h3 className="font-semibold text-lg">{t('extractedText')}</h3>
                              <button onClick={handleCopy} className="p-2 text-slate-500 hover:text-blue-600 rounded-full hover:bg-slate-100">
                                 <Clipboard size={18} />
                              </button>
                          </div>
                          <textarea
                              readOnly
                              value={ocrResult}
                              className="w-full p-4 bg-slate-100 rounded-lg text-sm"
                              rows={10}
                          />
                      </div>
                  )}
              </div>
          );
      };
      
      // =================================================================
      // TOOL: Screenshot Editor
      // =================================================================
      const ScreenshotEditor = () => {
          const [imageSrc, setImageSrc] = useState('');
          const [brushColor, setBrushColor] = useState('#FF0000');
          const [brushSize, setBrushSize] = useState(5);
          const canvasRef = useRef(null);
          const contextRef = useRef(null);
          const [isDrawing, setIsDrawing] = useState(false);
          const { t } = useTranslation();

          const handleFileAccepted = (file) => {
              const reader = new FileReader();
              reader.onload = (e) => {
                  if (e.target?.result) {
                      setImageSrc(e.target.result);
                  }
              };
              reader.readAsDataURL(file);
          };

          useEffect(() => {
              if (!imageSrc || !canvasRef.current) return;
              const canvas = canvasRef.current;
              const ctx = canvas.getContext('2d');
              const image = new window.Image();
              image.src = imageSrc;
              image.onload = () => {
                  canvas.width = image.width;
                  canvas.height = image.height;
                  ctx?.drawImage(image, 0, 0);
                  if (ctx) {
                      contextRef.current = ctx;
                  }
              };
          }, [imageSrc]);

          const startDrawing = ({ nativeEvent }) => {
              const { offsetX, offsetY } = nativeEvent;
              if (!contextRef.current) return;
              contextRef.current.beginPath();
              contextRef.current.moveTo(offsetX, offsetY);
              setIsDrawing(true);
          };

          const finishDrawing = () => {
              if (!contextRef.current) return;
              contextRef.current.closePath();
              setIsDrawing(false);
          };

          const draw = ({ nativeEvent }) => {
              if (!isDrawing || !contextRef.current) return;
              const { offsetX, offsetY } = nativeEvent;
              contextRef.current.lineTo(offsetX, offsetY);
              contextRef.current.strokeStyle = brushColor;
              contextRef.current.lineWidth = brushSize;
              contextRef.current.lineCap = 'round';
              contextRef.current.stroke();
          };

          const clearDrawing = () => {
              if (!imageSrc) return;
              const canvas = canvasRef.current;
              if (canvas) {
                  const ctx = canvas.getContext('2d');
                  const image = new window.Image();
                  image.src = imageSrc;
                  image.onload = () => {
                      ctx?.clearRect(0, 0, canvas.width, canvas.height);
                      ctx?.drawImage(image, 0, 0);
                  };
              }
          };
          
          const handleDownload = () => {
              if (!canvasRef.current) return;
              const link = document.createElement('a');
              link.download = 'screenshot-edited.png';
              link.href = canvasRef.current.toDataURL();
              link.click();
          };

          return (
              <div className="space-y-6">
                  {!imageSrc && <FileDropzone onFileAccepted={handleFileAccepted} acceptedFileTypes="image/jpeg, image/png, image/webp" />}
                  {imageSrc && (
                      <div className="flex flex-col items-center space-y-4">
                          <p className="text-center text-slate-600">{t('drawOnImage')}</p>
                          <div className="bg-slate-50 p-4 rounded-lg w-full max-w-lg flex flex-wrap items-center justify-center gap-4">
                              <div className="flex items-center gap-2">
                                  <Palette size={20} className="text-slate-600" />
                                  <label htmlFor="brushColor" className="text-sm font-medium">{t('brushColor')}</label>
                                  <input id="brushColor" type="color" value={brushColor} onChange={e => setBrushColor(e.target.value)} className="w-8 h-8"/>
                              </div>
                              <div className="flex items-center gap-2">
                                   <Pen size={20} className="text-slate-600" />
                                  <label htmlFor="brushSize" className="text-sm font-medium">{t('brushSize')}</label>
                                  <input id="brushSize" type="range" min="1" max="50" value={brushSize} onChange={e => setBrushSize(Number(e.target.value))} />
                              </div>
                               <Button onClick={clearDrawing} className="bg-slate-600 hover:bg-slate-700" icon={<Trash2 size={16}/>}>
                                  {t('clearDrawing')}
                              </Button>
                          </div>
                          <canvas
                              ref={canvasRef}
                              onMouseDown={startDrawing}
                              onMouseUp={finishDrawing}
                              onMouseMove={draw}
                              onMouseLeave={finishDrawing}
                              className="max-w-full h-auto rounded-lg shadow-md cursor-crosshair"
                              style={{maxHeight: '50vh'}}
                          />
                          <Button onClick={handleDownload} icon={<Download />}>{t('download')}</Button>
                      </div>
                  )}
              </div>
          );
      };

      // =================================================================
      // TOOL: YouTube Thumbnail Generator
      // =================================================================
      const YouTubeThumbnailGenerator = () => {
          const [title, setTitle] = useState('Your Awesome Title');
          const [bgColor, setBgColor] = useState('#007BFF');
          const [textColor, setTextColor] = useState('#FFFFFF');
          const [fontSize, setFontSize] = useState(80);
          const [bgImage, setBgImage] = useState(null);
          const canvasRef = useRef(null);
          const { t } = useTranslation();

          const drawCanvas = () => {
              const canvas = canvasRef.current;
              if (!canvas) return;
              const ctx = canvas.getContext('2d');
              if (!ctx) return;

              ctx.clearRect(0, 0, canvas.width, canvas.height);

              if (bgImage) {
                  ctx.drawImage(bgImage, 0, 0, canvas.width, canvas.height);
              } else {
                  ctx.fillStyle = bgColor;
                  ctx.fillRect(0, 0, canvas.width, canvas.height);
              }
              
              ctx.fillStyle = textColor;
              ctx.font = `bold ${fontSize}px 'Inter', sans-serif`;
              ctx.textAlign = 'center';
              ctx.textBaseline = 'middle';
              
              wrapText(ctx, title, canvas.width / 2, canvas.height / 2, canvas.width - 80, fontSize * 1.2);
          };

          useEffect(() => {
              drawCanvas();
          }, [title, bgColor, textColor, fontSize, bgImage]);
          
          const wrapText = (context, text, x, y, maxWidth, lineHeight) => {
              const words = text.split(' ');
              let line = '';
              const lines = [];

              for (let n = 0; n < words.length; n++) {
                  const testLine = line + words[n] + ' ';
                  const metrics = context.measureText(testLine);
                  const testWidth = metrics.width;
                  if (testWidth > maxWidth && n > 0) {
                      lines.push(line);
                      line = words[n] + ' ';
                  } else {
                      line = testLine;
                  }
              }
              lines.push(line);
              
              const startY = y - (lines.length - 1) * lineHeight / 2;

              for(let i = 0; i < lines.length; i++) {
                  context.fillText(lines[i], x, startY + i * lineHeight);
              }
          }


          const handleBgImageUpload = (e) => {
              if (e.target.files && e.target.files[0]) {
                  const reader = new FileReader();
                  reader.onload = (event) => {
                      const img = new window.Image();
                      img.onload = () => setBgImage(img);
                      img.src = event.target?.result;
                  };
                  reader.readAsDataURL(e.target.files[0]);
              }
          };
          
           const handleDownload = () => {
              if (!canvasRef.current) return;
              const link = document.createElement('a');
              link.download = 'youtube-thumbnail.png';
              link.href = canvasRef.current.toDataURL();
              link.click();
          };

          return (
              <div className="flex flex-col lg:flex-row gap-8">
                  <div className="lg:w-1/3 space-y-4">
                      <h3 className="font-semibold text-lg">{t('controls')}</h3>
                      <div className="space-y-2">
                          <label htmlFor="title" className="font-medium">{t('titleText')}</label>
                          <input id="title" type="text" value={title} onChange={e => setTitle(e.target.value)} className="w-full p-2 border-2 rounded-lg" />
                      </div>
                      <div className="space-y-2">
                          <label htmlFor="fontSize" className="font-medium">{t('fontSize')}: {fontSize}px</label>
                          <input id="fontSize" type="range" min="20" max="150" value={fontSize} onChange={e => setFontSize(Number(e.target.value))} className="w-full" />
                      </div>
                       <div className="space-y-2">
                          <label className="font-medium">{t('textColor')}</label>
                          <input type="color" value={textColor} onChange={e => setTextColor(e.target.value)} className="w-full h-10 p-1 border-2 rounded-lg" />
                      </div>
                       <div className="space-y-2">
                          <label className="font-medium">{t('backgroundColor')}</label>
                          <input type="color" value={bgColor} onChange={e => setBgColor(e.target.value)} className="w-full h-10 p-1 border-2 rounded-lg" disabled={!!bgImage} />
                      </div>
                       <div className="space-y-2">
                          <label className="font-medium">{t('uploadBackground')}</label>
                          <input type="file" onChange={handleBgImageUpload} accept="image/*" className="w-full text-sm file:mr-4 file:py-2 file:px-4 file:rounded-full file:border-0 file:text-sm file:font-semibold file:bg-blue-50 file:text-blue-700 hover:file:bg-blue-100"/>
                      </div>
                       <Button onClick={handleDownload} icon={<Download />} className="w-full">{t('download')}</Button>
                  </div>
                  <div className="lg:w-2/3">
                      <h3 className="font-semibold text-lg mb-2 text-center">{t('thumbnailPreview')}</h3>
                      <div className="aspect-video w-full bg-slate-200 rounded-lg shadow-lg overflow-hidden">
                          <canvas ref={canvasRef} width="1280" height="720" className="w-full h-full" />
                      </div>
                  </div>
              </div>
          );
      };

      // =================================================================
      // TOOL: Image to QR Code Reader
      // =================================================================
      const ImageToQRCode = () => {
          const [imageFile, setImageFile] = useState(null);
          const [imageUrl, setImageUrl] = useState('');
          const [decodedText, setDecodedText] = useState('');
          const [error, setError] = useState('');
          const canvasRef = useRef(null);
          const { t } = useTranslation();

          const handleFileAccepted = (file) => {
              setImageFile(file);
              setImageUrl(URL.createObjectURL(file));
              setDecodedText('');
              setError('');
          };

          useEffect(() => {
              if (!imageUrl || !canvasRef.current) return;
              
              const canvas = canvasRef.current;
              const ctx = canvas.getContext('2d');
              if (!ctx) return;
              
              const image = new window.Image();
              image.src = imageUrl;
              image.onload = () => {
                  canvas.width = image.width;
                  canvas.height = image.height;
                  ctx.drawImage(image, 0, 0, image.width, image.height);
                  const imageData = ctx.getImageData(0, 0, image.width, image.height);
                  const code = jsQR(imageData.data, imageData.width, imageData.height);

                  if (code) {
                      setDecodedText(code.data);
                      setError('');
                  } else {
                      setError(t('noQrCodeFound'));
                      setDecodedText('');
                  }
              };

          }, [imageUrl, t]);
          
          const handleCopy = () => {
              navigator.clipboard.writeText(decodedText);
          };

          return (
              <div className="space-y-6">
                  <canvas ref={canvasRef} className="hidden" />
                  {!imageFile && (
                      <FileDropzone onFileAccepted={handleFileAccepted} acceptedFileTypes="image/jpeg, image/png, image/webp" />
                  )}
                  
                  {imageFile && (
                       <div className="flex flex-col items-center">
                          <img src={imageUrl} alt="QR Code Preview" className="max-w-full h-auto rounded-lg shadow-md mx-auto" style={{ maxHeight: '300px' }} />
                      </div>
                  )}
                  
                  {error && (
                      <p className="text-center text-red-500 font-semibold">{error}</p>
                  )}
                  
                  {decodedText && (
                       <div className="space-y-2">
                          <h3 className="font-semibold text-lg">{t('decodedText')}</h3>
                          <div className="relative">
                              <textarea
                                  readOnly
                                  value={decodedText}
                                  className="w-full p-4 pr-12 bg-slate-100 rounded-lg text-sm"
                                  rows={4}
                              />
                               <button onClick={handleCopy} className="absolute top-2 right-2 p-2 text-slate-500 hover:text-blue-600 rounded-full hover:bg-slate-200">
                                 <Clipboard size={18} />
                              </button>
                          </div>
                      </div>
                  )}
              </div>
          );
      };

      // =================================================================
      // TOOL: Finance Calculator
      // =================================================================
      const FinanceCalculator = () => {
          const [activeTab, setActiveTab] = useState('emi');
          const { t } = useTranslation();

          const renderCalculator = () => {
              switch (activeTab) {
                  case 'emi':
                      return <EMICalculator />;
                  case 'simple':
                      return <SimpleInterestCalculator />;
                  case 'compound':
                      return <CompoundInterestCalculator />;
                  default:
                      return null;
              }
          };

          const tabs = [
              { id: 'emi', label: t('emiCalculator') },
              { id: 'simple', label: t('simpleInterest') },
              { id: 'compound', label: t('compoundInterest') },
          ];

          return (
              <div className="w-full max-w-xl mx-auto">
                  <div className="border-b border-slate-200 mb-6">
                      <nav className="-mb-px flex space-x-4" aria-label="Tabs">
                          {tabs.map(tab => (
                              <button
                                  key={tab.id}
                                  onClick={() => setActiveTab(tab.id)}
                                  className={`${
                                      activeTab === tab.id
                                          ? 'border-blue-500 text-blue-600'
                                          : 'border-transparent text-slate-500 hover:text-slate-700 hover:border-slate-300'
                                  } whitespace-nowrap py-4 px-1 border-b-2 font-medium text-sm transition-colors`}
                              >
                                  {tab.label}
                              </button>
                          ))}
                      </nav>
                  </div>
                  <div>{renderCalculator()}</div>
              </div>
          );
      };

      const EMICalculator = () => {
          const { t } = useTranslation();
          const [principal, setPrincipal] = useState('100000');
          const [rate, setRate] = useState('8.5');
          const [tenure, setTenure] = useState('10');
          const [emi, setEmi] = useState('');
          const [totalInterest, setTotalInterest] = useState('');
          const [totalAmount, setTotalAmount] = useState('');

          const calculateEMI = () => {
              const p = parseFloat(principal);
              const r = parseFloat(rate) / 12 / 100;
              const n = parseFloat(tenure) * 12;

              if (p > 0 && r > 0 && n > 0) {
                  const emiVal = (p * r * Math.pow(1 + r, n)) / (Math.pow(1 + r, n) - 1);
                  const totalAmt = emiVal * n;
                  const totalInt = totalAmt - p;
                  
                  setEmi(emiVal.toFixed(2));
                  setTotalAmount(totalAmt.toFixed(2));
                  setTotalInterest(totalInt.toFixed(2));
              }
          };
          
          return (
              <div className="space-y-4">
                  <Input label={t('principalAmount')} value={principal} onChange={e => setPrincipal(e.target.value)} />
                  <Input label={t('annualInterestRate')} value={rate} onChange={e => setRate(e.target.value)} />
                  <Input label={t('loanTenureYears')} value={tenure} onChange={e => setTenure(e.target.value)} />
                  <Button onClick={calculateEMI} className="w-full">{t('calculate')}</Button>
                  {emi && <Results data={[
                      { label: t('monthlyEMI'), value: emi },
                      { label: t('totalInterest'), value: totalInterest },
                      { label: t('totalAmount'), value: totalAmount },
                  ]} />}
              </div>
          );
      };

      const SimpleInterestCalculator = () => {
          const { t } = useTranslation();
          const [principal, setPrincipal] = useState('10000');
          const [rate, setRate] = useState('5');
          const [time, setTime] = useState('2');
          const [interest, setInterest] = useState('');
          const [totalAmount, setTotalAmount] = useState('');

          const calculate = () => {
              const p = parseFloat(principal);
              const r = parseFloat(rate) / 100;
              const t_val = parseFloat(time);

              if (p > 0 && r > 0 && t_val > 0) {
                  const intVal = p * r * t_val;
                  setInterest(intVal.toFixed(2));
                  setTotalAmount((p + intVal).toFixed(2));
              }
          };

          return (
               <div className="space-y-4">
                  <Input label={t('principalAmount')} value={principal} onChange={e => setPrincipal(e.target.value)} />
                  <Input label={t('annualInterestRate')} value={rate} onChange={e => setRate(e.target.value)} />
                  <Input label={t('timePeriodYears')} value={time} onChange={e => setTime(e.target.value)} />
                  <Button onClick={calculate} className="w-full">{t('calculate')}</Button>
                  {interest && <Results data={[
                      { label: t('totalInterest'), value: interest },
                      { label: t('totalAmount'), value: totalAmount },
                  ]} />}
              </div>
          );
      };

      const CompoundInterestCalculator = () => {
          const { t } = useTranslation();
          const [principal, setPrincipal] = useState('10000');
          const [rate, setRate] = useState('5');
          const [time, setTime] = useState('2');
          const [frequency, setFrequency] = useState(1);
          const [interest, setInterest] = useState('');
          const [totalAmount, setTotalAmount] = useState('');

          const calculate = () => {
              const p = parseFloat(principal);
              const r = parseFloat(rate) / 100;
              const t_val = parseFloat(time);
              const n = frequency;
              
              if(p > 0 && r > 0 && t_val > 0) {
                  const total = p * Math.pow(1 + r / n, n * t_val);
                  setTotalAmount(total.toFixed(2));
                  setInterest((total - p).toFixed(2));
              }
          };
          
          return (
               <div className="space-y-4">
                  <Input label={t('principalAmount')} value={principal} onChange={e => setPrincipal(e.target.value)} />
                  <Input label={t('annualInterestRate')} value={rate} onChange={e => setRate(e.target.value)} />
                  <Input label={t('timePeriodYears')} value={time} onChange={e => setTime(e.target.value)} />
                  <div>
                       <label className="block text-sm font-medium text-slate-700 mb-1">{t('compoundingFrequency')}</label>
                       <select value={frequency} onChange={e => setFrequency(Number(e.target.value))} className="w-full p-2 border-2 border-slate-200 rounded-lg">
                          <option value={1}>{t('annually')}</option>
                          <option value={2}>{t('semiAnnually')}</option>
                          <option value={4}>{t('quarterly')}</option>
                          <option value={12}>{t('monthly')}</option>
                       </select>
                  </div>
                  <Button onClick={calculate} className="w-full">{t('calculate')}</Button>
                  {interest && <Results data={[
                      { label: t('totalInterest'), value: interest },
                      { label: t('totalAmount'), value: totalAmount },
                  ]} />}
              </div>
          );
      };

      const Input = ({ label, value, onChange }) => (
          <div>
              <label className="block text-sm font-medium text-slate-700 mb-1">{label}</label>
              <input
                  type="number"
                  value={value}
                  onChange={onChange}
                  className="w-full p-2 border-2 border-slate-200 rounded-lg focus:outline-none focus:border-blue-500"
              />
          </div>
      );

      const Results = ({ data }) => (
          <div className="bg-blue-50 p-4 rounded-lg space-y-2 mt-4">
              {data.map(item => (
                  <div key={item.label} className="flex justify-between items-center">
                      <p className="text-slate-600">{item.label}</p>
                      <p className="font-bold text-blue-600 text-lg">₹ {Number(item.value).toLocaleString('en-IN')}</p>
                  </div>
              ))}
          </div>
      );
      
      // =================================================================
      // LIB: TOOLS CONFIG
      // =================================================================
      const tools = [
        {
          id: 'image-to-text',
          name: { en: 'Image to Text', hi: 'छवि से पाठ' },
          description: { en: 'Extract text from images using OCR.', hi: 'ओसीआर का उपयोग करके छवियों से पाठ निकालें।' },
          category: 'Image Tools',
          Icon: ScanText,
          component: ImageToText,
        },
        {
          id: 'image-compressor',
          name: { en: 'Image Compressor', hi: 'छवि कंप्रेसर' },
          description: { en: 'Reduce the file size of your images.', hi: 'अपनी छवियों का फ़ाइल आकार कम करें।' },
          category: 'Image Tools',
          Icon: ImageIcon,
          component: ImageCompressor,
        },
        {
          id: 'image-resizing',
          name: { en: 'Image Resizer', hi: 'छवि रिसाइज़र' },
          description: { en: 'Change the dimensions of your images.', hi: 'अपनी छवियों का आयाम बदलें।' },
          category: 'Image Tools',
          Icon: Milestone,
          component: ImageResizer,
        },
        {
          id: 'image-editor',
          name: { en: 'Image Editor', hi: 'छवि संपादक' },
          description: { en: 'Crop, filter, and edit your photos.', hi: 'अपनी तस्वीरों को काटें, फ़िल्टर करें और संपादित करें।' },
          category: 'Image Tools',
          Icon: Scissors,
          component: ImageEditor,
        },
        {
          id: 'screenshot-editor',
          name: { en: 'Screenshot Editor', hi: 'स्क्रीनशॉट संपादक' },
          description: { en: 'Annotate and edit your screenshots.', hi: 'अपने स्क्रीनशॉट को एनोटेट और संपादित करें।' },
          category: 'Image Tools',
          Icon: Edit,
          component: ScreenshotEditor,
        },
        {
          id: 'pdf-editor',
          name: { en: 'PDF Editor', hi: 'पीडीएफ संपादक' },
          description: { en: 'Edit and manage your PDF documents.', hi: 'अपने पीडीएफ दस्तावेजों को संपादित और प्रबंधित करें।' },
          category: 'Converter Tools',
          Icon: FileEdit,
          component: PlaceholderTool,
        },
        {
          id: 'video-editor',
          name: { en: 'Video Editor', hi: 'वीडियो संपादक' },
          description: { en: 'Trim, merge, and edit your videos.', hi: 'अपने वीडियो को ट्रिम, मर्ज और संपादित करें।' },
          category: 'Content Tools',
          Icon: Video,
          component: PlaceholderTool,
        },
        {
          id: 'youtube-title-generator',
          name: { en: 'YouTube Title Generator', hi: 'यूट्यूब शीर्षक जेनरेटर' },
          description: { en: 'Generate catchy titles for your videos.', hi: 'अपने वीडियो के लिए आकर्षक शीर्षक उत्पन्न करें।' },
          category: 'Content Tools',
          Icon: Youtube,
          component: YouTubeTitleGenerator,
        },
        {
          id: 'youtube-thumbnail-generator',
          name: { en: 'YouTube Thumbnail Generator', hi: 'यूट्यूब थंबनेल जेनरेटर' },
          description: { en: 'Create custom thumbnails for YouTube.', hi: 'यूट्यूब के लिए कस्टम थंबनेल बनाएं।' },
          category: 'Image Tools',
          Icon: GalleryThumbnails,
          component: YouTubeThumbnailGenerator,
        },
        {
          id: 'passport-photo-maker',
          name: { en: 'Passport Photo Maker', hi: 'पासपोर्ट फोटो मेकर' },
          description: { en: 'Create passport-sized photos easily.', hi: 'आसानी से पासपोर्ट आकार के फोटो बनाएं।' },
          category: 'Image Tools',
          Icon: ImageIcon,
          component: PassportPhotoMaker,
        },
        {
          id: 'image-to-qr-code',
          name: { en: 'Image to QR Code', hi: 'छवि से क्यूआर कोड' },
          description: { en: 'Scan and read QR codes from images.', hi: 'छवियों से क्यूआर कोड स्कैन और पढ़ें।' },
          category: 'Generators',
          Icon: QrCode,
          component: ImageToQRCode,
        },
        {
          id: 'text-to-qr-code',
          name: { en: 'Text to QR Code', hi: 'टेक्स्ट से क्यूआर कोड' },
          description: { en: 'Generate a QR code from any text.', hi: 'किसी भी टेक्स्ट से क्यूआर कोड जेनरेट करें।' },
          category: 'Generators',
          Icon: Type,
          component: TextToQRCode,
        },
        {
          id: 'finance-calculator',
          name: { en: 'Finance Calculator', hi: 'वित्त कैलकुलेटर' },
          description: { en: 'Calculate EMI, interest, and more.', hi: 'ईएमआई, ब्याज, और बहुत कुछ की गणना करें।' },
          category: 'Calculators',
          Icon: Landmark,
          component: FinanceCalculator,
        },
        {
          id: 'calculator',
          name: { en: 'Calculator', hi: 'कैलकुलेटर' },
          description: { en: 'A simple calculator for daily use.', hi: 'रोजमर्रा के उपयोग के लिए एक सरल कैलकुलेटर।' },
          category: 'Calculators',
          Icon: CalculatorIcon,
          component: AppCalculator,
        },
         {
          id: 'json-formatter',
          name: { en: 'JSON Formatter', hi: 'जेसन प्रारूपक' },
          description: { en: 'Format and validate your JSON data.', hi: 'अपने जेसन डेटा को प्रारूपित और मान्य करें।' },
          category: 'Content Tools',
          Icon: FileJson,
          component: JSONFormatter,
        },
      ];

      // =================================================================
      // COMPONENT: Header
      // =================================================================
      const Logo = () => (
          <div className="flex items-center space-x-2">
              <div className="p-2 bg-blue-500 rounded-lg">
                  <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="white" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round" className="w-6 h-6">
                      <path d="M14.7 6.3a1 1 0 0 0 0 1.4l1.6 1.6a1 1 0 0 0 1.4 0l3.77-3.77a6 6 0 0 1-7.94 7.94l-6.91 6.91a2.12 2.12 0 0 1-3-3l6.91-6.91a6 6 0 0 1 7.94-7.94l-3.76 3.76z"/>
                  </svg>
              </div>
              <span className="text-2xl font-bold text-slate-800">toolbox.ai</span>
          </div>
      );

      const ContactModal = ({onClose}) => {
          const { t } = useTranslation();
          return (
              <div className="fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center z-50 transition-opacity duration-300">
                  <div className="bg-white rounded-xl shadow-2xl p-8 w-full max-w-md m-4 transform transition-all duration-300 scale-95 opacity-0 animate-fade-in-scale">
                      <div className="flex justify-between items-center mb-6">
                          <h2 className="text-2xl font-bold text-slate-800">{t('contactInfo')}</h2>
                          <button onClick={onClose} className="text-slate-500 hover:text-slate-800 transition-colors">
                              <X size={24} />
                          </button>
                      </div>
                      <div className="space-y-4">
                          <a href="tel:7973831205" className="flex items-center space-x-4 p-4 rounded-lg hover:bg-slate-100 transition-colors">
                              <Phone className="text-blue-500" size={24} />
                              <div>
                                  <p className="font-semibold text-slate-600">{t('phone')}</p>
                                  <p className="text-lg text-slate-800">7973 831205</p>
                              </div>
                          </a>
                          <a href="mailto:vs1630365@gmail.com" className="flex items-center space-x-4 p-4 rounded-lg hover:bg-slate-100 transition-colors">
                              <Mail className="text-blue-500" size={24} />
                              <div>
                                  <p className="font-semibold text-slate-600">{t('email')}</p>
                                  <p className="text-lg text-slate-800">vs1630365@gmail.com</p>
                              </div>
                          </a>
                      </div>
                       <button onClick={onClose} className="mt-8 w-full bg-blue-500 text-white font-semibold py-3 rounded-lg hover:bg-blue-600 transition-colors focus:outline-none focus:ring-2 focus:ring-blue-500 focus:ring-opacity-50">
                          {t('close')}
                      </button>
                  </div>
                   <style>{`
                      @keyframes fade-in-scale {
                          0% { transform: scale(0.95); opacity: 0; }
                          100% { transform: scale(1); opacity: 1; }
                      }
                      .animate-fade-in-scale { animation: fade-in-scale 0.3s forwards; }
                  `}</style>
              </div>
          );
      };

      const Header = () => {
          const [isContactOpen, setContactOpen] = useState(false);
          const { language, setLanguage } = useLanguage();
          const { t } = useTranslation();

          return (
              <Fragment>
                  <header className="bg-white/80 backdrop-blur-lg shadow-sm sticky top-0 z-40">
                      <div className="container mx-auto px-4 py-4 flex justify-between items-center">
                          <Logo />
                          <nav className="flex items-center space-x-4">
                              <div className="relative group">
                                  <button className="flex items-center space-x-2 text-slate-600 hover:text-blue-500 transition-colors px-3 py-2 rounded-md">
                                      <Globe size={20} />
                                      <span>{language === 'en' ? 'English' : 'हिंदी'}</span>
                                  </button>
                                  <div className="absolute right-0 mt-2 w-36 bg-white rounded-md shadow-lg opacity-0 group-hover:opacity-100 transition-opacity duration-200 invisible group-hover:visible">
                                      <a onClick={() => setLanguage('en')} href="#" className={`block px-4 py-2 text-sm ${language === 'en' ? 'font-semibold text-blue-600 bg-blue-50' : 'text-slate-700'} hover:bg-slate-100`}>{t('english')}</a>
                                      <a onClick={() => setLanguage('hi')} href="#" className={`block px-4 py-2 text-sm ${language === 'hi' ? 'font-semibold text-blue-600 bg-blue-50' : 'text-slate-700'} hover:bg-slate-100`}>{t('hindi')}</a>
                                  </div>
                              </div>
                              <button 
                                  onClick={() => setContactOpen(true)}
                                  className="bg-blue-500 text-white font-semibold px-4 py-2 rounded-lg hover:bg-blue-600 transition-all duration-300 transform hover:scale-105"
                              >
                                  {t('contactUs')}
                              </button>
                          </nav>
                      </div>
                  </header>
                  {isContactOpen && <ContactModal onClose={() => setContactOpen(false)} />}
              </Fragment>
          );
      };

      // =================================================================
      // COMPONENT: Sidebar
      // =================================================================
      const Sidebar = ({ selectedCategory, onSelectCategory }) => {
        const { t } = useTranslation();

        const categories = [
          { id: 'all', name: t('allTools'), icon: LayoutGrid },
          { id: 'Image Tools', name: t('imageTools'), icon: ImageIcon },
          { id: 'Content Tools', name: t('contentTools'), icon: TypeIcon },
          { id: 'Converter Tools', name: t('converterTools'), icon: SlidersHorizontal },
          { id: 'Calculators', name: t('calculators'), icon: CalculatorIcon },
          { id: 'Generators', name: t('generators'), icon: Bot },
        ];

        return (
          <aside className="hidden lg:block w-64 bg-white p-4 rounded-xl shadow-sm">
            <nav className="space-y-2">
              {categories.map((category) => (
                <button
                  key={category.id}
                  onClick={() => onSelectCategory(category.id)}
                  className={`w-full flex items-center space-x-3 px-4 py-3 rounded-lg text-left transition-all duration-200 ${
                    selectedCategory === category.id
                      ? 'bg-blue-500 text-white shadow-md'
                      : 'text-slate-600 hover:bg-blue-50 hover:text-blue-600'
                  }`}
                >
                  <category.icon className="w-5 h-5" />
                  <span className="font-semibold">{category.name}</span>
                </button>
              ))}
            </nav>
          </aside>
        );
      };
      
      // =================================================================
      // COMPONENT: ToolGrid
      // =================================================================
      const ToolGrid = ({ tools: toolsToShow, searchTerm, setSearchTerm }) => {
          const { t, getLocalized } = useTranslation();
          const [activeTool, setActiveTool] = useState(null);

          const handleToolClick = (tool) => {
              setActiveTool(tool);
          };

          const handleCloseTool = () => {
              setActiveTool(null);
          };

          if (activeTool) {
              const ActiveToolComponent = activeTool.component;
              return (
                  <div className="bg-white p-6 md:p-8 rounded-xl shadow-lg animate-fade-in">
                      <div className="flex justify-between items-center mb-6">
                           <div className="flex items-center space-x-3">
                              <activeTool.Icon className="w-8 h-8 text-blue-500" />
                              <h2 className="text-2xl md:text-3xl font-bold text-slate-800">{getLocalized(activeTool.name)}</h2>
                          </div>
                          <button onClick={handleCloseTool} className="p-2 rounded-full hover:bg-slate-100 text-slate-500 hover:text-slate-800 transition-colors">
                              <X size={24} />
                          </button>
                      </div>
                      <ActiveToolComponent />
                  </div>
              );
          }

          return (
              <div className="w-full">
                  <div className="relative mb-8">
                      <Search className="absolute left-4 top-1/2 -translate-y-1/2 text-slate-400" />
                      <input
                          type="text"
                          value={searchTerm}
                          onChange={(e) => setSearchTerm(e.target.value)}
                          placeholder={t('searchTools')}
                          className="w-full pl-12 pr-4 py-4 bg-white border-2 border-transparent focus:border-blue-500 rounded-xl shadow-sm text-lg focus:outline-none transition-all"
                      />
                  </div>

                  {toolsToShow.length > 0 ? (
                      <div className="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 gap-6">
                          {toolsToShow.map(tool => (
                              <ToolCard key={tool.id} tool={tool} onClick={() => handleToolClick(tool)} />
                          ))}
                      </div>
                  ) : (
                      <div className="text-center py-16 text-slate-500">
                          <p>{t('noToolsFound')}</p>
                      </div>
                  )}
                   <style>{`
                      @keyframes fade-in {
                          from { opacity: 0; transform: translateY(10px); }
                          to { opacity: 1; transform: translateY(0); }
                      }
                      .animate-fade-in { animation: fade-in 0.3s ease-out forwards; }
                  `}</style>
              </div>
          );
      };
      
      // =================================================================
      // COMPONENT: ToolCard
      // =================================================================
      const ToolCard = ({ tool, onClick }) => {
        const { getLocalized } = useTranslation();
        
        return (
          <div 
            onClick={onClick}
            className="bg-white p-6 rounded-xl shadow-sm hover:shadow-lg hover:-translate-y-1 transition-all duration-300 cursor-pointer flex flex-col items-start h-full"
          >
            <div className="p-3 bg-blue-100 rounded-lg mb-4">
              <tool.Icon className="w-7 h-7 text-blue-600" />
            </div>
            <h3 className="font-bold text-lg text-slate-800 mb-2">{getLocalized(tool.name)}</h3>
            <p className="text-slate-500 text-sm flex-grow">{getLocalized(tool.description)}</p>
          </div>
        );
      };

      // =================================================================
      // COMPONENT: Footer
      // =================================================================
      const DonateModal = ({onClose}) => {
          const { t } = useTranslation();
          const upiId = "v86209644-1@okaxis";
          const upiLink = `upi://pay?pa=${upiId}&pn=Toolbox.ai&am=&cu=INR&tn=Donation%20for%20Toolbox.ai`;
          
          const qrCodePlaceholder = `https://api.qrserver.com/v1/create-qr-code/?size=200x200&data=${encodeURIComponent(upiLink)}`;

          return (
              <div className="fixed inset-0 bg-black bg-opacity-60 flex items-center justify-center z-50 transition-opacity duration-300">
                  <div className="bg-white rounded-xl shadow-2xl p-8 w-full max-w-sm m-4 text-center transform transition-all duration-300 scale-95 opacity-0 animate-fade-in-scale">
                      <div className="flex justify-between items-center mb-4">
                          <h2 className="text-2xl font-bold text-slate-800">{t('donateTitle')}</h2>
                          <button onClick={onClose} className="text-slate-500 hover:text-slate-800 transition-colors">
                              <X size={24} />
                          </button>
                      </div>
                      <p className="text-slate-600 mb-6">{t('donateDescription')}</p>
                      <div className="flex justify-center mb-4">
                           <img src={qrCodePlaceholder} alt="QR Code to donate" className="w-48 h-48 rounded-lg border-4 border-slate-200" />
                      </div>
                      <p className="font-semibold mb-6 text-slate-700">{t('scanToPay')}</p>
                      <a 
                          href={upiLink}
                          className="w-full inline-block bg-blue-500 text-white font-bold py-3 px-6 rounded-lg hover:bg-blue-600 transition-all transform hover:scale-105"
                      >
                          {t('payWithUPI')}
                      </a>
                  </div>
                   <style>{`
                      @keyframes fade-in-scale {
                          0% { transform: scale(0.95); opacity: 0; }
                          100% { transform: scale(1); opacity: 1; }
                      }
                      .animate-fade-in-scale { animation: fade-in-scale 0.3s forwards; }
                  `}</style>
              </div>
          );
      };

      const Footer = () => {
        const { t } = useTranslation();
        const [isDonateOpen, setDonateOpen] = useState(false);

        return (
          <Fragment>
            <footer className="bg-slate-900 text-white">
              <div className="container mx-auto px-4 py-8">
                <div className="grid grid-cols-1 md:grid-cols-3 gap-8 text-center md:text-left">
                  <div>
                    <h3 className="text-lg font-bold mb-4">toolbox.ai</h3>
                    <p className="text-slate-400">Your everyday online toolkit.</p>
                  </div>
                  <div className="flex flex-col space-y-2">
                     <a href="#" className="text-slate-300 hover:text-blue-400 transition-colors">{t('howToUse')}</a>
                     <a href="#" className="text-slate-300 hover:text-blue-400 transition-colors">{t('privacyPolicy')}</a>
                     <a href="#" className="text-slate-300 hover:text-blue-400 transition-colors">{t('contactUs')}</a>
                  </div>
                  <div className="flex flex-col items-center md:items-end space-y-4">
                      <button 
                          onClick={() => setDonateOpen(true)}
                          className="flex items-center space-x-2 bg-blue-500 text-white font-semibold px-6 py-3 rounded-lg hover:bg-blue-600 transition-all duration-300 transform hover:scale-105"
                      >
                          <Heart size={20} />
                          <span>{t('supportUs')}</span>
                      </button>
                  </div>
                </div>
                <div className="mt-8 border-t border-slate-700 pt-6 text-center text-slate-500">
                  &copy; {new Date().getFullYear()} toolbox.ai - {t('madeInIndia')} 🇮🇳
                </div>
              </div>
            </footer>
            {isDonateOpen && <DonateModal onClose={() => setDonateOpen(false)} />}
          </Fragment>
        );
      };
      
      // =================================================================
      // MAIN APP COMPONENT
      // =================================================================
      const App = () => {
          const [selectedCategory, setSelectedCategory] = useState('all');
          const [searchTerm, setSearchTerm] = useState('');

          const filteredTools = useMemo(() => {
              return tools.filter(tool => {
                  const categoryMatch = selectedCategory === 'all' || tool.category === selectedCategory;
                  const searchMatch = tool.name.en.toLowerCase().includes(searchTerm.toLowerCase()) || 
                                      tool.name.hi.toLowerCase().includes(searchTerm.toLowerCase()) ||
                                      tool.description.en.toLowerCase().includes(searchTerm.toLowerCase()) ||
                                      tool.description.hi.toLowerCase().includes(searchTerm.toLowerCase());
                  return categoryMatch && searchMatch;
              });
          }, [selectedCategory, searchTerm]);

          return (
              <LanguageProvider>
                  <div className="flex flex-col min-h-screen bg-slate-50 text-slate-800">
                      <Header />
                      <div className="flex flex-1 container mx-auto px-4 py-8">
                          <Sidebar selectedCategory={selectedCategory} onSelectCategory={setSelectedCategory} />
                          <main className="flex-1 lg:ml-8">
                              <ToolGrid tools={filteredTools} searchTerm={searchTerm} setSearchTerm={setSearchTerm} />
                          </main>
                      </div>
                      <Footer />
                  </div>
              </LanguageProvider>
          );
      };

      // =================================================================
      // RENDER APP
      // =================================================================
      const rootElement = document.getElementById('root');
      if (!rootElement) {
        throw new Error("Could not find root element to mount to");
      }

      const root = ReactDOM.createRoot(rootElement);
      root.render(
        <React.StrictMode>
          <App />
        </React.StrictMode>
      );
    </script>
  </body>
</html>
