# 1 Overview

ComPDFKit, a software development kit (SDK), consists of PDF SDK and PDF Conversion SDK. With ComPDFKit, even developers with limited knowledge of PDF can quickly integrate professional PDF functions with just a few lines of code on multiple platforms. And we will introduce ComPDFKit PDF SDK for Android here.

ComPDFKit PDF SDK for Android is a powerful PDF library for developers to add robust PDF functionality to their applications, which ships with simple-to-use java APIs to offer document viewing, creation, searching, annotation, and editing.

## 1.1 ComPDFKit PDF SDK

ComPDFKit PDF SDK consists of two elements as shown in the following picture.

![Alt text](https://github.com/ComPDFKit/PDF-SDK-Android/blob/main/image-android/ComPDFKit.png)

The two elements for ComPDFKit PDF SDK:

- **PDF Core API**

  A parser for PDF documents (also known as PDF Data layer) doesn’t include any UI components. If you just need to render a PDF document without displaying any content inside the PDF, you can just integrate this into your application.

- **PDF View**

  The rendering library for PDF documents (also known as the PDF UI layer) relies on **ComPDFKit-UI.aar**. It is a visual operation logic package for page rendering, annotation operations, and form operations. You can customize page rendering and operations based on the file library.

## 1.2 Key Features

**Viewer** component offers: 

- Standard page display modes, including Scrolling, Double page, Crop mode, and Cover mode.
- Navigation with thumbnails, outlines, and bookmarks.
- Text search & selection.
- Zoom in and out.
- Switch between different themes, including Dark mode, Sepia mode, Reseda mode, and Custom color mode.
- Text reflow.

**Annotations** component offers:

- Create, edit and remove annotations, including Notes, Link, Freetext, Line, Square, Circle, Highlight, Underline, Squiggly, Strikeout, Ink, and Stamp.
- Support for annotation appearances.
- Import and export annotations to/from XFDF.
- Support for annotation flattening.

**Forms** component offers:

- Create, edit and remove form fields, including Push Button, Check Box, Radio Button, Text Field, Combo Box, List Box, and Signature.
- Fill PDF Forms.
- Support for PDF form flattening.

**Document editor** component offers:

- PDF manipulation, including Split pages, Extract pages, and Merge pages.
- Page edit, including Delete pages, Insert pages, Move pages, Rotate pages, Replace pages, and Exchange pages.
- Access document information.
- Extract images.

**Security** component offers:

- Encrypt and decrypt PDFs, including Permission setting and Password protected.
- Create, edit, and remove watermark.
- Redact content including images, text, and vector graphics.
- Create, edit, and remove header & footer, including dates, page numbers, document name, author name, and chapter name.
- Create, edit, and remove bates numbers.
- Create, edit, and remove background that can be a solid color or an image.

**Conversion** component offers:

- PDF to PDF/A.

## 1.3 License

ComPDFKit PDF SDK is a commercial SDK, which requires a license to grant developer permission to release their apps. Each license is only valid for one application ID in development mode. Other flexible licensing options are also supported, please contact [our marketing team](mailto:support@compdf.com) to know more.  However, any documents, sample code, or source code distribution from the released package of ComPDFKit PDF SDK to any third party is prohibited.

# 2 Get Started

It is easy to embed  ComPDFKit PDF SDK in your Android application with a few lines of Java code. Takes just a few minutes and gets started. 

The following sections introduce the structure of the installation package, how to run a demo, and how to make an Android app in Java with ComPDFKit PDF SDK.

## 2.1 Requirements

ComPDFKit PDF SDK is supported on Android devices running API level 19 or newer and targeting the latest stable Android version 4.4 or higher. Furthermore, ComPDFKit PDF SDK requires apps to enable Java 8 language features to build.

- Android Studio 3.2 or newer (support AndroidX).
- Project specifications.
  - A `minSdkVersion` of `19` or higher.
  - A `compileSdkVersion` of `30` or higher.
  - A `targetSdkVersion` of `30` or higher.
  - Android ABI(s): x86, x86_64, armeabi-v7a, arm64-v8a.

## 2.2 Android Package Structure

The package of ComPDFKit PDF SDK for Android includes the following files as shown in Figure 2-1:

- **libs** - A folder containing **ComPDFKit.aar**, **ComPDFKit-UI.aar**, and **ComPDFKit-Utils.aar**. **ComPDFKit.aar** is PDF Core API. **ComPDFKit-UI.aar** is PDF View. **ComPDFKit-Utils.aar** includes UI extensions component based on the fundamental layout classes: `ReaderFragment` or `ReaderActivity`.
- **PDFViewer** - A folder containing Android sample projects.
- **api_reference_android** - API reference.
- **developer_guide_android.pdf** - Developer guide.
- **release_notes.txt** - Release information.
- **legal.txt** - Legal and copyright information.

![Alt text](https://github.com/ComPDFKit/PDF-SDK-Android/blob/main/image-android/2.2.png)

<p align="center">
Figure 2-1
</p>

## 2.3 How to Run a Demo 

ComPDFKit PDF SDK for Android provides one demo in Java for developers to learn how to call the SDK on Android. You can find them in the ***"PDFViewer"*** folder. In this guide, it takes the "Java" demo as an example to show how to run it in Android.

1. Import the ***"PDFViewer"*** project on Android Studio.
2. In the toolbar, select ***"PDFViewer"*** from the run configurations drop-down menu.
3. From the target device drop-down menu, select the device that you want to run ***"ComPDFKit_Demo"*** on.
4. Click ***"Run"***.

If you don't have any devices configured, then you need to either connect a device via USB or create an AVD to use the Android Emulator.

![Alt text](https://github.com/ComPDFKit/PDF-SDK-Android/blob/main/image-android/2.3.png)

**Note:** *This is a demo project, presenting completed ComPDFKit PDF SDK functions. The functions might be different based on the license you have purchased. Please check that the functions you choose work fine in this demo project.*
