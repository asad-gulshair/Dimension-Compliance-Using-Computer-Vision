# Dimension-Compliance-Using-Computer-Vision
This project focuses on dimension compliance inspection of disk-shaped objects using computer vision. The system automatically measures the inner and outer diameters of disks and compares them against defined standards.
To ensure accurate and scale-consistent measurements, ArUco markers are used as reference objects in images.

Key Features

Automated Diameter Measurement

Detects and measures both inner and outer diameters.

Annotation Pipeline

Collected image samples and annotated them for training.

ArUco Marker Integration

Ensures real-world unit measurement by using markers as scale references.

Dimension Compliance Check

Measured values can be compared with standard tolerances (e.g., ASME, ISO).

Tech Stack

Python

OpenCV (for image processing, contour detection, ArUco marker detection)

YOLO / Object Detection (for disk and region localization)

NumPy & Pandas (for calculations & reporting)

Dataset & Annotation

Images of disk samples were collected under controlled conditions.

Each image contains an ArUco marker for scaling.

Annotations include:

Outer boundary (disk edge)

Inner boundary (hole/center cut)

Measurement Workflow

Detect ArUco marker → calculate pixel-to-mm ratio.

Detect disk edges using segmentation / bounding boxes.

Measure inner & outer diameters in millimeters.

Compare results against standard specifications.

Example Output

Input: Disk image with ArUco marker

Output:

Outer Diameter: XX mm

Inner Diameter: YY mm

Compliance: ✅ Pass / ❌ Fail

Future Improvements

Integrate more flange types and disk variants.

Build a real-time inspection system with video input.

Develop a web dashboard for compliance reporting.

Contribution

Contributions are welcome!

Fork the repo

Create a feature branch

Submit a pull request 

License

This project is licensed under the MIT License.
