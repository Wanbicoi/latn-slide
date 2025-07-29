```
UNIVERSITY OF SCIENCE
HONOR PROGRAM IN COMPUTER SCIENCE
```
```
LE LONG TRUONG THINH - HOANG THE TRUNG
```
# ANNOTATION SYSTEM FOR MEDICAL DATA

# WITH SMART ASSISTANCE

```
BACHELOR OF SCIENCE IN COMPUTER SCIENCE
```
```
HO CHI MINH CITY, 2025
```

```
UNIVERSITY OF SCIENCE
HONOR PROGRAM IN COMPUTER SCIENCE
```
##### LE LONG TRUONG THINH 21125079

##### HOANG THE TRUNG 21120583

# ANNOTATION SYSTEM FOR MEDICAL DATA

# WITH SMART ASSISTANCE

```
BACHELOR OF SCIENCE IN COMPUTER SCIENCE
```
##### THESIS ADVISOR

##### ASSOC. PROF. TRẦN MINH TRIẾT

```
M.Sc. Đỗ Trọng Lễ
```
```
HO CHI MINH CITY, 2025
```

```
ACKNOWLEDGEMENT
```
We would like to extend our sincere gratitude to Associate Professor Tran Minh
Triet and M.Sc. Do Trong Le for their dedicated guidance and continuous sup-
port throughout our undergraduate studies. Their mentorship has been instru-
mental in nurturing our academic development and inspiring us to pursue re-
search with curiosity and determination. Their encouragement and valuable ad-
vice have accompanied us through every stage of this thesis.

We are especially thankful to Dr. Dao Thi Phuong Thao for her generous support
in providing essential medical data and professional healthcare knowledge, which
have been crucial to the successful execution of our project. Her expertise has
greatly enriched our understanding of the medical domain and helped us apply
our research in a meaningful and practical context.

Our appreciation also goes to all the lecturers of the Faculty of Information
Technology, University of Science, VNU-HCM, whose outstanding teaching and
dedication to academic excellence have laid a strong foundation for our stud-
ies. Their insightful lectures and guidance have equipped us with the necessary
knowledge and skills for academic and research success.

We are grateful to our friends for their constant support, constructive feedback,
and enthusiastic encouragement, all of which have made this challenging journey
more enjoyable and rewarding. Their contributions have helped improve the
quality of our work in many ways.

Our special thanks also go to the Software Engineering Laboratory (SELab),
University of Science, VNU-HCM, for providing excellent research facilities and
technical assistance that enabled us to successfully complete our thesis.

Finally, we are deeply indebted to our families for their unconditional love, pa-


tience, and endless encouragement. Their support has been a pillar of strength,
allowing us to overcome difficulties and remain focused on achieving our aca-
demic goals with confidence and determination.


```
TABLE OF CONTENTS
```
```
Page
```
Acknowledgement ................................................................

Table of Contents ................................................................

Abstract........................................................................... ii

##### CHAPTER 1 – INTRODUCTION

1.1 Problem Overview ......................................................... 1

1.2 Objectives and Contributions............................................. 2

```
1.2.1 Primary Objectives................................................. 2
1.2.2 Specific Contributions ............................................. 2
1.2.3 Scope and Limitations ............................................. 3
```
1.3 Thesis Organization ....................................................... 4

CHAPTER 2 – LITERATURE REVIEW AND RELATED
WORK

2.1 Medical Data Annotation Techniques.................................... 6

```
2.1.1 Traditional Medical Annotation Methods........................ 6
2.1.2 DICOM Standards and Medical Imaging Infrastructure........ 6
2.1.3 Challenges in Medical Annotation ................................ 7
```
2.2 Current Annotation Support Systems ................................... 8

```
2.2.1 Comparative Analysis of Current Systems ....................... 8
```

## CHAPTER 3 – PROBLEM ANALYSIS AND PROPOSED



   - 2.2.2 OHIF Viewer Platform
   - 2.2.3 MONAI Label Framework
   - 2.2.4 Encord and Commercial Workflow Management
   - 2.2.5 Orthanc and DICOM-Based Data Management
- 2.3 AI in Medical Annotation.................................................
   - 2.3.1 Interactive Segmentation Techniques
   - 2.3.2 Foundation Models in Medical Imaging
- 2.4 Workflow Management in Healthcare
   - 2.4.1 Task Assignment and Tracking Systems
   - 2.4.2 Quality Control Processes
   - 2.4.3 Collaboration Tools and Communication
- 2.5 Research Gap Analysis
   - 2.5.1 Limitations of Current Approaches
   - 2.5.2 Integration and Interoperability Gaps............................
   - 2.5.3 Opportunities for Innovation
- 3.1 Approach to System Development SOLUTION
- 3.2 Detailed Problem Analysis
   - 3.2.1 Traditional Medical Annotation Workflow Analysis
   - 3.2.2 Expert Knowledge and Time Challenges.........................
   - 3.2.3 Consistency and Quality Control Issues..........................
   - 3.2.4 Collaboration and Communication Barriers
   - 3.2.5 Stakeholder Analysis and Requirements
- 3.3 Proposed Solution Overview
   - 3.3.1 Integrated Intelligent Annotation System Concept
   - 3.3.2 Core System Components
- 4.1 System Architecture Overview CHAPTER 4 – DETAILED SYSTEM DESIGN
- 4.2 Frontend Architecture
   - 4.2.1 Accelerating Development with a Headless Framework.........
      - 4.2.1.1 Problem: Boilerplate and Scaffolding Overhead
      - 4.2.1.2 Solution: Adoption of the Refine.dev Framework......
   - 4.2.2 Efficient Data Caching and State Synchronization..............
         - Inconsistency 4.2.2.1 Problem: Inefficient Data Fetching and UI
         - Invalidation with TanStack Query 4.2.2.2 Solution: Declarative Caching and Automated
- 4.3 Backend Architecture and Workflow Orchestration
   - 4.3.1 Secure and Abstracted Data Access via Views and Functions
         - Duplication 4.3.1.1 Problem: Direct Table Exposure and Logic
         - PostgreSQL Views and Functions....................... 4.3.1.2 Solution: A Multi-Layered Abstraction with
   - 4.3.2 Asynchronous Workflow Automation Engine
         - Transitions 4.3.2.1 Problem: Orchestrating Non-Interactive Workflow
      - 4.3.2.2 Solution: A Cron-Based, Database-Centric Engine....
      - 4.3.2.3 Operational Flow and State Transition.................
- 4.4 OHIF–MONAI Integrated Interface and Operational Workflow
   - 4.4.1 Overview of integrated architecture
   - 4.4.2 Main Function
   - 4.4.3 Annotation Process
- 4.5 Infrastructure and Security
   - 4.5.1 Unified Authentication Across Micro-Frontends.................
      - 4.5.1.1 Problem: Disparate Authentication States
         - Reverse Proxy............................................. 4.5.1.2 Solution: Centralized Authentication via Nginx
- 5.1 Evaluation Methodology and Results CHAPTER 5 – EXPERIMENTATION AND EVALUATION
   - 5.1.1 Research Context and Study Design
   - 5.1.2 Evaluation Criteria
      - 5.1.2.1 Annotation Workflow Efficiency
      - 5.1.2.2 Quality and Benefit of AI Assistance
      - 5.1.2.3 User Experience and Collaboration.
- 5.2 Experimental Results
- 5.3 Evaluation Summary


##### CHAPTER 6 – CONCLUSION AND FUTURE WORK

6.1 Summary of Contributions................................................ 64

6.2 Remaining Limitations .................................................... 65

6.3 Future Works............................................................... 66

6.4 Closing Remarks ........................................................... 66

References ...................................................................... 67

```
i
```

```
ABSTRACT
```
Medical image annotation remains a critical bottleneck in healthcare AI, de-
manding extensive expertise and manual labor, significantly constraining the
scalability and effectiveness of AI solutions in clinical environments. Based on
real-world challenges encountered during deployment in Vietnamese hospitals,
this thesis proposes an intelligent annotation system specifically designed to
integrate AI effectively into clinical annotation workflows, thus substantially
reducing manual workload and improving the efficiency and quality of data la-
beling.

The developed system is structured into four main integrated components: (1)
a workflow management platform built with React [1] and Supabase [2], facili-
tating structured collaboration, clear task delegation, detailed permissions, and
interactive feedback mechanisms between doctors and annotation staff; (2) an
annotation interface integrated within OHIF Viewer 3.x [3], providing intuitive
visual tools supported by advanced AI assistance; (3) an AI module powered
by MONAI Label [4], further optimized with foundation models such as the Seg-
ment Anything Model (SAM) [5] and U-Net [6] to achieve precise multi-organ
segmentation; and (4) Orthanc PACS for secure, standardized storage and man-
agement [7, 8] of medical images in DICOM format.

The key innovations of this thesis lie in three principal contributions: (1) im-
plementing a structured, multi-stage annotation workflow thatstitchestogether
heterogeneous open-source platforms (Encord for task orchestration, OHIF for
visualisation, MONAI Label for AI inference, and Orthanc for DICOM storage),
leverages their respective strengths through additional custom code, and em-
beds clear collaboration and reviewer-feedback loops so that senior radiologists
can audit and guide junior annotators efficiently [9, 10]; (2) optimizing AI seg-
mentation models to achieve operational efficiency while maintaining clinically
acceptable accuracy, aided by interactive refinement techniques; and (3) con-

```
ii
```

ducting rigorous practical evaluations within a real clinical setting, specifically
at Thong Nhat Hospital, to demonstrate the system’s viability and readiness for
broader hospital adoption.

Ultimately, this research seeks to contribute practical, scalable solutions that
empower healthcare institutions, particularly in resource-limited environments,
to effectively leverage AI, transforming the medical annotation process toward
greater accuracy, productivity, and clinical relevance.

```
iii
```

```
CHAPTER 1
INTRODUCTION
```
```
This chapter establishes why high-quality, expertly annotated medical
images are a bottleneck for AI in Vietnamese hospitals and frames
the thesis around solving that problem. It (1) summarizes the practi-
cal obstacles—manual, siloed, low-AI annotation workflows; (2) states
four concrete objectives for building an integrated, AI-assisted plat-
form with scalable workflow management; (3) highlights three distinc-
tive contributions: expert-centred workflow design, lightweight yet ac-
curate AI integration, and real-world clinical validation; (4) clarifies
the study’s scope (CT/MRI DICOM data) and current limitations
(single-site evaluation); and (5) maps the six-chapter structure of the
dissertation, showing how subsequent chapters move from literature
and problem analysis to system design, implementation, evaluation,
and future work.
```
1.1 Problem Overview

With the growing demand for high-quality, annotated medical imaging datasets
crucial for healthcare AI applications, hospitals in Vietnam currently struggle
with inefficient manual annotation processes, fragmented team coordination, and
limited integration of advanced AI technologies. These challenges not only hinder
data quality but also place significant burdens on medical experts, ultimately
limiting the scalability and effectiveness of AI-driven clinical tools. Addressing
these challenges requires an intelligent annotation system that seamlessly inte-
grates advanced AI with structured workflow management, enabling enhanced
productivity, annotation accuracy, and collaboration.


1.2 Objectives and Contributions

1.2.1 Primary Objectives

This thesis aims to develop a comprehensive intelligent annotation system to
resolve the highlighted issues effectively. The primary objectives guiding this
research include:

Objective 1: Develop an Integrated Annotation PlatformConstruct an
integrated platform combining advanced medical imaging visualization capabil-
ities and AI-powered annotation tools to streamline complex annotation tasks
for medical professionals.

Objective 2: Implement AI-Assisted SegmentationDeploy and optimize
advanced AI segmentation tools, including foundation models like SAM and
interactive refinement techniques, to assist clinicians in accurately identifying
and segmenting anatomical structures and pathologies.

Objective 3: Design Flexible Workflow Management Create a robust
workflow management system supporting diverse annotation processes, clearly
defined roles, quality control mechanisms, and dynamic collaboration scenarios
involving direct medical expert engagement.

Objective 4: Ensure System Scalability and IntegrationDesign a scalable
system architecture readily integrable with existing clinical infrastructures such
as PACS systems, adhering strictly to DICOM standards, thus ensuring broader
adoption potential across various clinical settings.

1.2.2 Specific Contributions

This thesis distinctly emphasizes three principal contributions:

Enhanced Expert-driven Workflow Management: The research intro-


duces a comprehensive workflow management system facilitating structured task
assignment, clear multi-stage annotation processes, and direct involvement from
medical experts (doctors). The system also incorporates real-time collaboration,
enabling instant feedback, communication, and expert validation to enhance an-
notation quality and operational efficiency.

Optimized AI Model Integration: Significant effort is dedicated to opti-
mizing advanced AI models (e.g., customized UNET architectures and SAM
foundation models) to balance computational efficiency and clinical accuracy.
The integration of interactive refinement methods further ensures the annota-
tion quality aligns closely with clinical standards, minimizing manual correction
efforts.

Real-world Clinical Evaluation and Deployment:The developed system
has been rigorously tested and evaluated at Thong Nhat Hospital in Vietnam.
Real-world clinical validation and expert-driven feedback have ensured practi-
cal applicability, relevance, and readiness for broader hospital implementation,
directly addressing operational challenges in Vietnamese healthcare contexts.

1.2.3 Scope and Limitations

Scope of Research:The research primarily targets CT and MRI medical im-
ages in DICOM format, focusing on prevalent annotation tasks such as organ
segmentation, lesion detection, and anatomical labeling, tailored explicitly for
deployment within Vietnamese healthcare environments.

Research Limitations:Current system validation is restricted to Thong Nhat
Hospital, influencing the AI model’s effectiveness due to dependence on locally
available training data. Operational validation is similarly constrained by the
specific workflow practices of this institution, suggesting potential future adap-
tations required for broader deployment scenarios.


1.3 Thesis Organization

This thesis is structured into six chapters, each addressing a specific aspect of
the research:

Chapter 1: Introduction outlines the research context, clearly defining ob-
jectives and emphasizing the three principal contributions.

Chapter 2: Literature Review and Related Workexamines existing meth-
ods, identifying gaps in current annotation practices and establishing the theo-
retical framework for the proposed approach.

Chapter 3: Problem Analysis and Proposed Solutionprovides a detailed
analysis of current challenges and presents the intelligent annotation system
architecture as a comprehensive solution.

Chapter 4: Detailed System Designelaborates on technical implementa-
tions, including architecture, modules, technological choices, and integration
methodologies.

Chapter 5: Experimentation and Evaluationpresents the system’s deploy-
ment in a real hospital environment, assessing performance, user feedback, and
integration with clinical workflows.

Chapter 6: Conclusion and Future Work summarizes key contributions,
limitations encountered, and future research directions, underscoring the sys-
tem’s potential clinical impact.

Technical appendices supplement the thesis with detailed specifications, user
guidelines, and additional deployment insights for future development and op-
erational enhancements.


```
CHAPTER 2
LITERATURE REVIEW AND RELATED WORK
```
This chapter lays the scholarly groundwork for this thesis by sur-
veying and critiquing five key knowledge areas. It opens with a por-
trait of traditional expert-driven annotation—slice-by-slice inspection,
hierarchical quality checks, and the unavoidable drawbacks of time,
cost, and inter-observer inconsistency. The discussion then moves to
DICOM standards and imaging infrastructure, showing how Struc-
tured Reports, Segmentation Objects, and DICOMweb APIs create
the technical bridge between humans and machines. Next, a com-
parative review of four representative systems—OHIF, MONAI La-
bel, Encord, and Orthanc—highlights where each platform excels and
where it falls short for building an end-to-end intelligent workflow. A
fourth section surveys modern AI techniques, from interactive segmen-
tation modes (auto, point-prompt, class-prompt) to foundation models
such as SAM, and pairs these advances with best practices in clin-
ical workflow management—skill-based task assignment, multi-stage
quality gates, and real-time collaboration tools. The chapter closes
with a research-gap analysis that synthesises the unresolved issues:
fragmented toolchains, limited AI integration, scalability hurdles, and
PACS interoperability gaps. Those gaps provide the rationale for the
unified, AI-assisted, multi-stage workflow proposed in the following
chapters.


2.1 Medical Data Annotation Techniques

2.1.1 Traditional Medical Annotation Methods

Medical image annotation has traditionally relied on manual processes performed
by expert radiologists and medical professionals. These conventional approaches
have formed the foundation of medical imaging interpretation for decades and
continue to be the gold standard for accuracy and reliability.

Manual Annotation Workflows:Traditional medical annotation involves ra-
diologists examining medical images slice by slice, identifying anatomical struc-
tures, pathological findings, and regions of interest. This process typically in-
cludes contouring organs, marking lesions, measuring distances, and providing
descriptive annotations. The workflow generally follows a systematic approach
where experts review images in multiple planes (axial, sagittal, and coronal) to
ensure comprehensive coverage and accuracy.

Expert-Based Quality Control: Conventional annotation workflows incor-
porate multiple levels of review, often involving senior radiologists validating
annotations made by junior colleagues or residents. This hierarchical approach
ensures quality but significantly increases the time and cost associated with
annotation processes.

Standardization Efforts:Medical communities have developed various stan-
dardization protocols to ensure consistency in annotation practices. These in-
clude anatomical atlases, standardized terminology systems such as RadLex, and
institutional guidelines that aim to reduce inter-observer variability.

2.1.2 DICOM Standards and Medical Imaging Infrastructure

The Digital Imaging and Communications in Medicine (DICOM) standard plays
a crucial role in medical imaging annotation by providing a comprehensive frame-


work for storing, transmitting, and managing medical images and associated
metadata.

DICOM Structure and Annotation Support: DICOM supports various
types of annotations through specialized objects such as DICOM Structured
Reports (SR), DICOM Segmentation Objects, and DICOM Presentation States.
These standardized formats enable interoperability between different medical
imaging systems and ensure that annotations can be consistently interpreted
across various platforms and institutions.

DICOM Segmentation Objects:Modern DICOM standards include support
for storing segmentation results as DICOM objects, enabling the preservation of
automated and manual segmentation results within the standard medical imag-
ing workflow. This capability is essential for integrating AI-assisted annotation
tools with existing medical imaging infrastructure.

Structured Reporting:DICOM Structured Reports provide a standardized
mechanism for storing complex annotation data, including measurements, ob-
servations, and diagnostic conclusions. This format enables machine-readable
storage of annotation results while maintaining human readability and clinical
relevance.

2.1.3 Challenges in Medical Annotation

Medical image annotation faces several significant challenges that limit its effi-
ciency and scalability:

Complexity and Expertise Requirements: Medical images contain com-
plex anatomical structures with subtle variations that require extensive medical
training to interpret accurately. The need for specialized knowledge creates a
bottleneck in annotation workflows, as qualified experts are limited and expen-
sive.


Inter-observer Variability:Studies have consistently shown significant vari-
ability between different experts annotating the same medical images. This vari-
ability can impact the quality of datasets used for training AI models and affect
the reproducibility of research results.

Time and Resource Constraints: Manual annotation is extremely time-
consuming, with complex cases requiring hours of expert time. This limitation
severely restricts the scale at which annotated medical datasets can be created,
hindering the development of large-scale AI applications in healthcare.

2.2 Current Annotation Support Systems

2.2.1 Comparative Analysis of Current Systems

```
Table 2.1: Comparison of Current Annotation Support Systems
Feature OHIF Viewer MONAI La-
bel
```
```
Encord Orthanc
Medical Imag-
ing Support
```
```
Excellent Good Limited Excellent
AI Assistance None Excellent Limited None
Workflow Man-
agement
```
```
Basic None Excellent None
DICOM Inte-
gration
```
```
Excellent Good None Excellent
Collaborative
Features
```
```
Limited None Excellent None
Customization High High Limited High
```
The analysis reveals that while each system excels in specific areas, no sin-
gle platform provides comprehensive coverage of all requirements for intelligent
medical annotation workflows.


### 2.2.2 OHIF Viewer Platform

The Open Health Imaging Foundation (OHIF) Viewer represents one of the
most successful open-source platforms for web-based medical image viewing and
annotation.

Architecture and Capabilities: OHIF Viewer is built as a progressive web
application using modern JavaScript frameworks, enabling deployment across
various platforms without requiring specialized software installation. The plat-
form supports multi-modal medical imaging data and provides comprehensive
tools for image visualization, measurement, and annotation.

DICOM Compliance and Integration:OHIF Viewer provides extensive sup-
port for DICOM standards, including DICOMweb protocols for data retrieval
and storage. This compliance enables seamless integration with existing Picture
Archiving and Communication Systems (PACS) and medical imaging infrastruc-
ture commonly found in healthcare institutions.

Extensibility and Customization:The platform’s modular architecture al-
lows for extensive customization and extension through a plugin system. This
flexibility has made OHIF Viewer popular for research applications and custom
medical imaging solutions.

Limitations and Gaps:While OHIF Viewer provides excellent visualization
capabilities, it lacks built-in AI assistance features and sophisticated workflow
management tools. The platform requires significant customization to support
complex annotation workflows and collaborative features needed for large-scale
annotation projects.


### 2.2.3 MONAI Label Framework

MONAI Label represents a significant advancement in AI-assisted medical im-
age annotation, providing a comprehensive framework for integrating machine
learning models into annotation workflows.

```
Figure 2.1: AI-Innotation with model SAM-2D
```
AI-Assisted Annotation Capabilities: MONAI Label incorporates state-
of-the-art deep learning models for automatic and interactive segmentation of
medical images. The framework supports various AI models, including foun-
dation models like SAM2D, interactive segmentation tools like DeepEdit, and
specialized models for specific anatomical structures.

Interactive Segmentation Approach: The framework implements interac-
tive segmentation techniques that allow users to guide AI models through point
clicks, bounding boxes, and partial annotations. This approach combines the
efficiency of automated segmentation with the precision of expert guidance.

Model Training and Adaptation: MONAI Label includes capabilities for
continuous learning and model adaptation based on user corrections and feed-


back. This feature enables the system to improve over time and adapt to specific
institutional requirements and annotation styles.

Integration Challenges:While MONAI Label provides powerful AI capabili-
ties, its integration with existing medical imaging workflows and PACS systems
requires significant technical expertise. The framework primarily focuses on the
AI components and lacks comprehensive workflow management and user inter-
face components needed for complete annotation solutions.

### 2.2.4 Encord and Commercial Workflow Management

Encord represents the commercial state-of-the-art in annotation workflow man-
agement, providing comprehensive tools for managing large-scale annotation
projects.

```
Figure 2.2: Overview of Encord Active
```
Workflow Management Features: Encord provides sophisticated workflow
management capabilities including task assignment, progress tracking, quality
control processes, and collaborative annotation features. The platform supports


complex annotation pipelines with multiple review stages and automated quality
assurance mechanisms.

Quality Control and Validation:The platform includes comprehensive qual-
ity control features such as inter-annotator agreement metrics, automated qual-
ity checks, and hierarchical review processes. These features help ensure anno-
tation consistency and accuracy across large teams and projects.

Collaboration and Team Management:Encord supports advanced collabo-
ration features including real-time annotation sharing, team management tools,
and communication features that facilitate coordination among distributed an-
notation teams.

Limitations for Medical Applications: While Encord provides excellent
general-purpose annotation management capabilities, it lacks specific features
required for medical imaging applications such as DICOM integration, medical-
specific annotation tools, and compliance with healthcare regulatory require-
ments.

### 2.2.5 Orthanc and DICOM-Based Data Management

Orthanc serves as a powerful and lightweight open-source DICOM server, pro-
viding essential infrastructure for managing medical imaging data in intelligent
annotation systems. It is widely adopted for its ability to store, organize, and
facilitate access to DICOM-compliant images in both research and clinical envi-
ronments.


```
Figure 2.3: Orthanc Viewer - Storage Data for Patient
```
DICOM Storage and Access: Orthanc acts as the central repository for
patient imaging studies, storing both image data and associated metadata in
compliance with DICOM standards. It supports full-featured DICOMweb APIs,
enabling seamless data retrieval and integration with front-end viewers like OHIF
and AI inference backends like MONAI Label.

Integration with OHIF and MONAI Label:In an integrated annotation
system, Orthanc enables OHIF Viewer to stream medical images directly via
DICOMweb, providing radiologists and annotators with a web-based viewing
experience. Simultaneously, MONAI Label accesses the same data source to run
AI-powered segmentation or classification tasks, enabling a synchronized and
efficient AI-assisted annotation workflow.

Collaborative Data Management:Orthanc supports secure upload and mod-
ification of imaging datasets, allowing senior radiologists or project administra-
tors to manage data lifecycle efficiently. Through built-in access controls and
plugins, users can upload new studies, modify metadata, or delete outdated
data as required, making Orthanc a collaborative hub rather than just a passive


archive.

Limitations and Customization Needs:While Orthanc excels in DICOM
storage and interoperability, it does not provide native tools for workflow man-
agement or annotation UI. To function effectively in modern annotation plat-
forms, it must be integrated with complementary tools such as OHIF, MONAI
Label, and workflow orchestration systems.

## 2.3 AI in Medical Annotation.................................................

### 2.3.1 Interactive Segmentation Techniques

Interactive segmentation represents a paradigm shift in medical image anno-
tation, combining the efficiency of automated algorithms with the precision of
expert guidance.

Point-Based Interaction Methods:Modern interactive segmentation tech-
niques allow users to guide segmentation algorithms through simple point clicks
indicating foreground and background regions. These methods, such as those
implemented in DeepEdit, enable rapid refinement of automated segmentation
results with minimal user effort.

Scribble-Based Approaches:Advanced interactive methods support scribble-
based input where users can draw rough outlines or corrections that guide
the segmentation algorithm. This approach is particularly effective for complex
anatomical structures where point-based methods may be insufficient.

Bounding Box and Geometric Constraints: Some interactive segmenta-
tion methods utilize geometric constraints such as bounding boxes, ellipses, or
other geometric primitives to guide the segmentation process. These methods
are particularly useful for well-defined anatomical structures with predictable
shapes.


### 2.3.2 Foundation Models in Medical Imaging

Recent advances in foundation models have revolutionized the landscape of med-
ical image analysis and annotation.

SAM and Medical Foundation Models:SAM (Segment Anything Model)
represents a breakthrough in medical imaging AI, providing a versatile founda-
tion model capable of segmenting diverse anatomical structures across various
medical imaging modalities. With its zero-shot segmentation capabilities and in-
teractive prompt-based approach, this model significantly reduces the need for
specialized model training for each anatomical structure or imaging protocol.

Transfer Learning and Adaptation:Foundation models enable efficient adap-
tation to new medical imaging tasks through transfer learning approaches. This
capability allows the rapid deployment of AI assistance for new anatomical re-
gions or pathological conditions without requiring extensive training data.

Zero-Shot and Few-Shot Learning: Advanced foundation models demon-
strate zero-shot and few-shot learning capabilities, enabling annotation assis-
tance for previously unseen anatomical structures or rare pathological conditions
with minimal training examples.

## 2.4 Workflow Management in Healthcare

### 2.4.1 Task Assignment and Tracking Systems

Effective workflow management in medical annotation requires sophisticated
task assignment and tracking capabilities that account for the specialized nature
of medical expertise and the critical importance of annotation quality.

Expertise-Based Assignment:Medical annotation workflows must consider
the specific expertise and qualifications of annotators when assigning tasks. Dif-
ferent medical specialties may be required for different types of imaging studies


or anatomical regions.

Workload Balancing:Effective systems must balance workload across avail-
able annotators while considering factors such as case complexity, annotator
experience, and quality requirements. This balancing is crucial for maintaining
consistent productivity and quality across large annotation projects.

Progress Monitoring:Comprehensive tracking systems provide real-time vis-
ibility into annotation progress, quality metrics, and potential bottlenecks. This
information enables project managers to make informed decisions about resource
allocation and timeline adjustments.

### 2.4.2 Quality Control Processes

Quality control in medical annotation requires specialized processes that ensure
both accuracy and consistency while maintaining reasonable throughput.

Multi-Stage Review Processes:Medical annotation workflows typically in-
corporate multiple review stages, including initial annotation, expert review, and
final validation. Each stage may involve different levels of expertise and different
quality criteria.

Automated Quality Checks:Modern systems incorporate automated quality
checks that can identify potential errors or inconsistencies in annotations. These
checks may include geometric consistency validation, anatomical plausibility as-
sessment, and comparison with reference standards.

Inter-Annotator Agreement Metrics:Quality control systems must provide
mechanisms for measuring and tracking inter-annotator agreement, enabling
identification of cases requiring additional review or consensus building.


### 2.4.3 Collaboration Tools and Communication

Effective collaboration tools are essential for managing distributed annotation
teams and facilitating communication between annotators, reviewers, and project
managers.

Real-Time Collaboration Features:Modern annotation platforms support
real-time collaboration features that enable multiple experts to work simultane-
ously on the same case or to provide immediate consultation and feedback.

Communication and Annotation History:Comprehensive systems main-
tain detailed histories of annotation activities, including comments, revisions,
and communication between team members. This information is crucial for main-
taining annotation quality and resolving disagreements.

Knowledge Sharing Platforms:Advanced collaboration systems include knowl-
edge sharing features such as annotation guidelines, reference cases, and best
practice documentation that help maintain consistency across large annotation
teams.

## 2.5 Research Gap Analysis

### 2.5.1 Limitations of Current Approaches

The analysis of existing medical annotation systems reveals several significant
limitations that create opportunities for improvement:

Fragmented Solutions:Current solutions typically excel in specific areas but
fail to provide comprehensive coverage of all annotation workflow requirements.
Users must integrate multiple systems, leading to complexity and inefficiency.

Limited AI Integration:While AI-assisted annotation tools exist, their in-
tegration with comprehensive workflow management and collaborative features


remains limited. Most systems treat AI assistance as an add-on rather than a
core component of the annotation workflow.

Scalability Challenges:Many current solutions struggle with scalability, ei-
ther in terms of the number of users, the volume of data, or the complexity of
annotation workflows. This limitation restricts their applicability to large-scale
annotation projects.

Customization Complexity:While many systems offer customization capa-
bilities, the complexity of implementing and maintaining customizations often
exceeds the capabilities of healthcare institutions, limiting adoption and effec-
tiveness.

### 2.5.2 Integration and Interoperability Gaps............................

Current medical annotation systems suffer from significant integration and in-
teroperability challenges:

PACS Integration Complexity:While many systems claim PACS compati-
bility, the practical implementation of seamless integration with existing hospital
infrastructure remains challenging and often requires significant technical exper-
tise.

Data Format Inconsistencies: Different systems use varying data formats
and standards for storing annotations, making it difficult to transfer annotations
between systems or maintain long-term accessibility.

Workflow Incompatibility: Existing systems often impose their own work-
flow paradigms, making it difficult to adapt them to established institutional
practices and procedures.


### 2.5.3 Opportunities for Innovation

The identified limitations create several opportunities for innovative solutions:

Unified Platform Development: There is a clear need for a unified plat-
form that integrates medical image viewing, AI-assisted annotation, workflow
management, and collaborative features into a cohesive solution.

Adaptive AI Integration:Opportunities exist for developing more sophisti-
cated AI integration approaches that adapt to institutional requirements and
learn from user interactions over time.

Simplified Deployment and Maintenance:There is significant value in de-
veloping solutions that can be easily deployed and maintained by healthcare
institutions without requiring extensive technical expertise.

Enhanced Interoperability: Developing solutions with enhanced interoper-
ability features that can seamlessly integrate with existing healthcare infras-
tructure would significantly increase adoption and effectiveness.

The research presented in this thesis addresses these opportunities by developing
an integrated intelligent annotation system that combines the strengths of exist-
ing approaches while addressing their limitations through innovative integration
and design approaches.


```
CHAPTER 3
PROBLEM ANALYSIS AND PROPOSED SOLUTION
```
```
This chapter serves as the hinge between the introductory context
and the detailed design that follows. It begins by analysing the cur-
rent medical-image annotation workflow on three levels: (1) expos-
ing technical bottlenecks in speed, collaboration, and quality control;
(2) describing human-resource challenges such as the shortage of ex-
pert annotators, heavy time demands, and inconsistent labelling; and
(3) translating stakeholder expectations—especially those of radiol-
ogists—into a concise set of functional and non-functional require-
ments. Building on that analysis, the chapter then outlines the pro-
posed solution: a single intelligent annotation platform that fuses four
complementary technologies (Encord for workflow orchestration, OHIF
for image interaction, MONAI Label for AI assistance, and Orthanc
for DICOM storage). By combining a multi-stage, expert-centred work-
flow with lightweight interactive AI and built-in collaboration, the so-
lution directly addresses the identified pain points. The chapter con-
cludes by introducing the four core components and explaining how
they work together, laying the groundwork for the architectural and
implementation details presented in the next chapter.
```
3.1 Approach to System Development

To ensure the final platform answered genuine clinical needs while remaining
technically feasible, we adopted aniterativeandincremental development life-
cycle. Each iteration consisted of four tightly-coupled steps:

```
1.Stakeholder workshopswith radiologists, technicians, and hospital IT
staff to elicit concrete pain points and to validate early mock-ups.
```

```
2.Rapid prototypingof a minimal slice of functionality (e.g. a basic OHIF
viewer plug-in or a draft workflow screen) using short, two-week sprints.
3.In-clinic feedbacktogether with the radiologists we uploaded an anonymised
dataset—curated and supplied by the doctors themselves—to a sandbox
PACS instance. While the clinicians explored the prototype, they docu-
mented comments on usability, speed, and AI accuracy; the development
team concurrently captured these observations and consolidated them into
actionable items for the next improvement cycle.
4.Incremental refinement in which lessons from the previous cycle were
folded back into revised requirements, leading either to further polishing
or to re-prioritisation of the backlog.
```
The complete system architecture has already been illustrated in Figure 4.1
(Chapter 4). That diagram shows how the four principal blocks—Workflow
UI, OHIF Viewer, MONAI Label AI Engine, and Orthanc PACS—are unified
through the Supabase backend and an Nginx reverse proxy. Within the scope of
Chapter 3 we emphasise two major phases emerged from this process:

- Phase 1 – Problem Analysis: Mapping the legacy annotation flow
    end-to-end, classifying delays (sequential processing, isolated work, limited
    QC), and quantifying resource constraints (expert scarcity, annotation fa-
    tigue).
- Phase 2 – Solution Proposal: Designing a single platform that fuses
    workflow orchestration (Encord), image interaction (OHIF), AI assistance
    (MONAI Label), and secure DICOM storage (Orthanc), all surfaced through
    a React + Supabase stack.

Technical specifics—including access control, RLS policies, and AI interaction


flow—are analysed in depth in Chapter 4.

## 3.2 Detailed Problem Analysis

### 3.2.1 Traditional Medical Annotation Workflow Analysis

The traditional medical annotation workflow presents several critical bottlenecks
that significantly impact the efficiency and scalability of medical AI develop-
ment. Through analysis of current practices in Vietnamese healthcare institu-
tions and international standards, we have identified key problematic areas that
require systematic addressing.

Sequential Processing Bottlenecks:Current annotation workflows follow a
strictly sequential approach where medical images must be processed one by one
by individual experts. This approach creates significant throughput limitations,
as the annotation capacity is directly constrained by the number of available
expert annotators and their working hours.

Isolated Work Environment:Medical professionals typically work in isolation
when performing annotations, lacking real-time collaboration tools and immedi-
ate access to colleagues for consultation. This isolation leads to increased decision
time for complex cases and reduces the opportunity for knowledge sharing and
consensus building.

Lack of AI Assistance Integration:While AI tools for medical imaging exist,
they are rarely integrated into clinical annotation workflows. Medical profession-
als must manually export data, run separate AI tools, and then manually import
results back into their annotation environment, creating friction that discourages
adoption.

Inadequate Progress Tracking: Current systems provide limited visibility
into annotation progress, quality metrics, and resource utilization. This lack


of transparency makes it difficult for project managers to optimize workflows,
allocate resources effectively, or predict completion timelines.

### 3.2.2 Expert Knowledge and Time Challenges.........................

The dependence on expert medical knowledge creates fundamental scalability
challenges that cannot be resolved through traditional approaches alone.

Knowledge Scarcity and Geographical Distribution:Specialized medical
imaging expertise is unevenly distributed, with many healthcare institutions,
particularly in developing regions like Vietnam, having limited access to expert
radiologists and medical imaging specialists. This scarcity creates significant bot-
tlenecks in annotation workflows and limits the ability to develop comprehensive
medical AI systems.

Training Time and Cost:Developing medical imaging expertise requires years
of specialized training and continuous education to stay current with evolving
medical knowledge and imaging technologies. The high cost and time investment
required to train qualified annotators creates a significant barrier to scaling
annotation operations.

Cognitive Load and Fatigue Management: Medical image annotation is
cognitively demanding work that requires sustained attention and decision-making.
Extended annotation sessions often lead to decreased accuracy and increased er-
ror rates, necessitating careful workload management and break scheduling that
further reduces overall throughput.

Specialization Requirements:Different types of medical imaging studies re-
quire different areas of expertise. A radiologist specializing in chest imaging may
not be qualified to annotate brain MRI studies, creating additional constraints
on task assignment and resource allocation.


### 3.2.3 Consistency and Quality Control Issues..........................

Maintaining consistent annotation quality across large datasets and multiple
annotators presents significant challenges that impact the reliability of resulting
AI models.

Inter-Annotator Variability:Studies have consistently demonstrated signif-
icant variability between different experts annotating the same medical images
[11]. This variability can range from 10-30% disagreement rates even among ex-
perienced radiologists, creating inconsistencies that negatively impact AI model
training and validation [12].

Intra-Annotator Consistency:Individual annotators may exhibit inconsis-
tency over time due to factors such as fatigue, learning, or changes in interpre-
tation criteria. This temporal variability adds another layer of complexity to
quality control processes.

Lack of Real-Time Quality Feedback: Traditional annotation workflows
provide limited real-time feedback on annotation quality, making it difficult
to identify and correct errors or inconsistencies promptly [10]. Quality issues
are often discovered only during post-annotation review processes, leading to
expensive rework.

Standardization Challenges:While medical communities have developed var-
ious standardization guidelines, implementing and maintaining consistent adher-
ence to these standards across distributed annotation teams remains challenging,
particularly in resource-constrained environments.

### 3.2.4 Collaboration and Communication Barriers

Effective medical annotation often requires collaboration and communication
between multiple experts, but current systems provide limited support for these


activities.

Asynchronous Communication Delays:When annotators need consultation
or clarification, current systems typically rely on email or phone communication,
creating delays and interrupting workflow continuity. These delays can signifi-
cantly impact overall annotation throughput and quality.

Lack of Shared Context:When experts communicate about specific annota-
tion cases, they often lack shared visual context, making it difficult to convey
precise information about anatomical structures or pathological findings. This
limitation can lead to misunderstandings and suboptimal annotation decisions.

Knowledge Isolation: Annotation decisions and rationale are typically not
captured or shared systematically, leading to isolation of valuable medical knowl-
edge that could benefit other annotators working on similar cases.

Version Control and Change Tracking:Current systems provide limited ca-
pabilities for tracking annotation changes, maintaining version history, or under-
standing the evolution of annotation decisions over time. This limitation makes
it difficult to learn from annotation processes and improve future workflows.

### 3.2.5 Stakeholder Analysis and Requirements

Primary Stakeholders - Radiologists and Medical Imaging Specialists

Radiologists and medical imaging specialists represent the core users and benefi-
ciaries of the proposed intelligent annotation system. These stakeholders interact
with the system in multiple capacities, including providing imaging data, anno-
tating medical images, and validating annotation quality.

As Medical Image Data Providers, radiologists require seamless integration
of the annotation system with existing PACS and medical imaging infrastruc-
tures already established within hospitals. Ensuring full compliance with the


DICOM standard is critical for their daily workflows, as it facilitates effortless
data exchange and interoperability across diverse imaging modalities. Addition-
ally, radiologists prioritize secure and compliant data handling mechanisms to
maintain patient privacy and data integrity. Efficient tools for importing new
imaging studies and exporting annotated data sets for clinical and research pur-
poses are also necessary to streamline the entire annotation lifecycle.

In their role as Expert Annotators, radiologists expect high-quality visual-
ization capabilities that closely align with their familiar clinical workflows. The
annotation interface must be intuitive and enable easy interaction, leveraging
advanced AI assistance designed explicitly to complement and enhance, rather
than replace, their medical judgment. These specialists particularly value an-
notation tools that automate routine segmentation tasks, significantly reducing
manual effort and allowing more focus on complex clinical decisions. Moreover,
effective collaborative annotation features are essential, enabling them to consult
colleagues in real-time on challenging cases, thereby enhancing overall annota-
tion accuracy and confidence.

Finally, as Quality Validators and Reviewers, radiologists require robust,
built-in mechanisms for quality control and validation throughout the anno-
tation process. Clear and structured workflows for reviewing, commenting on,
and approving annotations are essential to uphold clinical accuracy and reliabil-
ity standards. Comprehensive progress tracking and project management tools
are also needed to facilitate timely oversight and resource allocation. Lastly,
comprehensive training resources and responsive technical support materials are
essential to ensure smooth system adoption, allowing clinical teams to leverage
the full capabilities of the annotation platform effectively.


## 3.3 Proposed Solution Overview

### 3.3.1 Integrated Intelligent Annotation System Concept

To effectively overcome the challenges identified in clinical annotation workflows,
we propose the development of an integrated intelligent annotation system that
unifies key capabilities into a single, scalable solution. This design is grounded in
practical experience from real-world deployments in Vietnamese hospitals and
directly addresses the limitations of current practices.

Unified Platform Approach:Instead of requiring clinicians to juggle multiple
disconnected tools, the proposed system offers a unified platform that seamlessly
integrates medical image viewing, AI-assisted annotation, structured workflow
management, and real-time collaboration. This integration reduces operational
friction and simplifies clinical deployment—ensuring that medical staff can work
efficiently within a cohesive environment tailored to their daily needs.

Workflow-Centric with Expert Involvement:A core innovation of the sys-
tem is its structured, multi-stage annotation workflow—designed to involve med-
ical experts meaningfully throughout the process. Doctors and senior specialists
participate not only in annotation but also in task validation, feedback, and qual-
ity control, ensuring clinical accuracy. This addresses the bottleneck of isolated
annotation and promotes reliability through expert consensus and structured
oversight.

Intelligent AI-Assisted Support:The system leverages state-of-the-art AI
models—particularly SAM and UNET via the MONAI Label framework—to
offer context-aware, interactive segmentation. These models provide zero-shot
or few-shot suggestions that annotators can refine using intuitive prompts such
as clicks or class labels. This approach significantly reduces manual workload
while maintaining high clinical standards, embodying the principle of AI as an


assistant—not a replacement—for medical professionals.

Clinical Readiness and Deployment-Oriented Design:Unlike many the-
oretical solutions, this system has been rigorously evaluated in a real-world hos-
pital setting—specifically Thong Nhat Hospital—validating its effectiveness, us-
ability, and integration potential. Feedback from practicing radiologists informed
key design decisions, ensuring that the system is not only technically sound but
also practically viable for broader adoption across healthcare institutions, espe-
cially in resource-limited environments.

Collaborative by Design: Collaboration features are embedded from the
ground up, supporting real-time multi-user annotation, role-specific access, and
contextual communication between team members. This mitigates the common
problem of expert isolation, promotes shared understanding, and enables better
annotation quality through team-based review and consensus mechanisms.

### 3.3.2 Core System Components

Component 1: Workflow Management Platform

The workflow management platform serves as the central orchestration layer re-
sponsible for coordinating annotation activities and managing system resources
across the entire pipeline. It supports project creation, configuration, and dy-
namic workflow definitions that accommodate various annotation paradigms.
Key capabilities include automated task assignment based on user availability
and specialization, real-time progress monitoring, role-based access control, and
integrated communication features to ensure seamless collaboration across dis-
tributed teams.

From a technical standpoint, this component is implemented as a React-based
web application utilizing the Refine.dev framework, backed by Supabase for
real-time database functionality. PostgreSQL is employed as the primary data


storage solution with an optimized schema tailored to medical workflows. The
platform is designed following a RESTful API architecture to allow integration
with external systems and future scalability.

Component 2: OHIF Annotation Interface

The annotation interface provides clinicians and annotation staff with an intu-
itive and powerful environment for interacting with medical images while lever-
aging AI-powered assistance. It supports advanced DICOM-compliant image
visualization and integrates OHIF Viewer 3.x with MONAI Label to deliver real-
time intelligent annotation. Users are offered two modes: manual annotation for
expert-level precision and AI-assisted annotation for accelerated workflows. Fea-
tures such as interactive auto-segmentation, point prompts, and class prompts
allow users to iteratively refine results. The interface also supports collabora-
tive annotations with multi-user sessions, annotation versioning, a commenting
system for feedback, and customizable layouts to suit radiologists’ preferences.

Technically, this component builds upon OHIF Viewer 3.x, with added enhance-
ments via Cornerstone3D for high-performance rendering. Integration with the
MONAI Label server is achieved through RESTful APIs, enabling bidirectional
communication with AI models. Custom extensions are implemented to facil-
itate both manual and AI-assisted annotation modes, while real-time updates
and collaboration features are supported by a persistent database-backed review
and feedback system.

Component 3: AI Assistance Engine (MONAI Label Server)

The AI assistance engine delivers intelligent support for annotation tasks by
incorporating state-of-the-art medical imaging models. It supports foundation
models for multi-organ segmentation, interactive segmentation methods such as


DeepEdit, and model-in-the-loop learning. Additional capabilities include uncer-
tainty quantification, annotation quality scoring, and custom model integration
for site-specific tuning. The engine also allows for batch processing and automa-
tion of repetitive annotation tasks, significantly improving throughput.

This component is built using the MONAI Label framework and leverages Py-
Torch for model implementation and inference. It is packaged within Docker
containers for scalable deployment and supports GPU acceleration to ensure re-
sponsive real-time inference. The modular design enables easy replacement or
updating of AI models as clinical needs evolve.

Component 4: Medical Data Management System (Orthanc PACS)

The medical data management system ensures secure, DICOM-compliant stor-
age and access to imaging data. It acts as the centralized image repository and
integrates seamlessly with hospital Picture Archiving and Communication Sys-
tems (PACS). Core functionalities include DICOMweb access for interoperabil-
ity, automatic extraction and indexing of metadata, data backup and archival,
and performance optimization for handling large volumes of imaging studies.

Orthanc serves as the underlying PACS engine, offering robust DICOM storage
and retrieval services. Lua scripting is employed for custom automation and in-
tegration logic, while a PostgreSQL backend manages metadata. RESTful APIs
expose programmatic access to stored datasets, enabling smooth data exchange
between components and external clinical systems.

The proposed solution provides a comprehensive foundation for intelligent med-
ical annotation that addresses the identified challenges while enabling future
enhancement and adaptation to evolving medical annotation needs. The de-
tailed technical architecture and implementation strategies are presented in the
following chapter.


```
CHAPTER 4
DETAILED SYSTEM DESIGN
```
```
This chapter provides a comprehensive exposition of the system’s de-
tailed design, articulating the architectural decisions, methodologies,
and technological implementations that underpin the platform. The
design philosophy centers on leveraging a modern, serverless archi-
tecture to achieve scalability, maintainability, and rapid development.
Each section adopts a problem-solution paradigm, presenting a spe-
cific technical challenge encountered during the development lifecycle,
followed by a detailed description of the implemented solution, its ra-
tionale, and its advantages.
```
4.1 System Architecture Overview

The platform’s architecture is a system comprising several loosely coupled com-
ponents, orchestrated to deliver a seamless data annotation experience. The
high-level architecture, as depicted in Figure 4.1, segregates responsibilities into
four primary domains: the client-side frontend, the serverless backend, external
service integrations, and a reverse proxy layer for routing and security.


```
Figure 4.1: High-Level System Architecture Diagram.
```
The frontend is a single-page application (SPA) built with React, responsible
for all user interactions. The backend is implemented entirely on the Supabase
platform, utilizing its PostgreSQL database, authentication services, and real-


time capabilities. This backend-as-a-service (BaaS) model obviates the need for
traditional server management. Key external integrations, such as the OHIF
Viewer for DICOM rendering and MONAI Label for AI-assisted annotation, are
incorporated to provide specialized functionality. An Nginx reverse proxy serves
as the entry point to the system, managing request routing and centralizing
authentication concerns. The subsequent sections will deconstruct this architec-
ture, providing a granular analysis of each component’s design.

## 4.2 Frontend Architecture

The frontend architecture is engineered for rapid development, maintainabil-
ity, and a high-quality user experience. The design addresses two fundamental
challenges in modern web application development: the overhead of building
standard application features and the complexity of client-side state manage-
ment.

### 4.2.1 Accelerating Development with a Headless Framework.........

#### 4.2.1.1 Problem: Boilerplate and Scaffolding Overhead

Developing a data-intensive application from the ground up necessitates a dis-
proportionate amount of engineering effort dedicated to repetitive, boilerplate
code rather than unique business features. For each distinct data entity—such
as projects,tasks, or users—a developer must manually implement a full
suite of standard features. This includes a view to list all items, a form to create
new ones, views to display and edit item details, and the logic to delete them.
This pattern, commonly known as Create, Read, Update, Delete (CRUD), ex-
tends beyond data operations to include user authentication flows (login, logout,
registration), system notifications, navigation menus, and breadcrumbs.

Without a structured framework, this leads to a proliferation of nearly identical


```
yet subtly different code blocks. A developer might write a custom React hook
for fetching project data, another for task data, and so on. Each implementation
would require its own state management (useState), effect handling (useEffect),
and API call logic. This approach is not only exceedingly time-consuming but
also highly susceptible to inconsistencies in implementation, error handling, and
loading state management, ultimately degrading code quality and maintainabil-
ity.
```
#### 4.2.1.2 Solution: Adoption of the Refine.dev Framework......

The platform leverages the refine.dev framework, a headless, React-based
framework designed specifically to abstract these common application patterns.
Its core architectural concept is theresource, a declarative object that defines
a data entity and its associated behaviors.
By defining a resource, the developer providesrefine.devwith the metadata
required to automate a vast array of functionalities. A resource definition for
"projects" is as follows:
1 <Refine
2 dataProvider ={...}
3 notificationProvider ={...}
4 routerProvider ={...}
5 authProvider ={...}
6 resources ={[
7 {
8 name: "projects",
9 list: "/projects",
10 create: "/projects/create",
11 edit: "/projects/edit/:id",


12 show: "/projects/show/:id",
13 meta: { canDelete: true }
14 },
15 _// ... other resources like "tasks", "users"_
16 ]}
17 >
18 { _/* Application components */_ }
19 </Refine >

```
This single, declarative definition unlocks a suite of powerful, interconnected
features, forming the backbone of the application:
```
- Standardized Data Hooks provide high-level data hooks (useList,useOne,
    useCreate,useUpdate,useDelete) that are pre-configured to communi-
    cate with the backend dataProvider. This eliminates the need to write
    manual fetching logic for each resource.
- Automated Routing enables the framework to generate necessary routes
    for thelist,create,edit, andshowpages, integrating seamlessly with
    itsrouterProvider.
- Dynamic UI Generation works with UI libraries like Ant Design where
    refine.devautomatically generates side-menu navigation links and bread-
    crumbs for each resource, ensuring a consistent and intuitive user experi-
    ence.
- Integrated Authentication leverages the framework’sauthProviderto han-
    dle login/logout flows and protect routes, redirecting unauthenticated users
    automatically.
- Centralized Notifications leverage thenotificationProviderto dispatch
    system-wide notifications for success or error events during data operations.


This resource-centric paradigm abstracts away the low-level implementation de-
tails of application infrastructure. It enabled the development team to bypass
thousands of lines of boilerplate code and focus engineering effort on high-value,
domain-specific features.

### 4.2.2 Efficient Data Caching and State Synchronization..............

4.2.2.1 Problem: Inefficient Data Fetching and UI Inconsistency

Managing server state—data fetched from a remote source—is a formidable chal-
lenge in any complex SPA. Without a sophisticated caching strategy, applica-
tions suffer from poor performance, redundant network traffic, and UI inconsis-
tencies. Two common anti-patterns demonstrate this problem:

```
1.Component-Level Fetching and Request Waterfalls: The most di-
rect approach involves each component fetching its own data using ‘useEf-
fect‘. This leads to perceptible latency as a parent component fetches data,
and then its child components, upon rendering, initiate their own separate
data fetches. Furthermore, if multiple unrelated components on the same
page require the same data (e.g., the current user’s profile), they will each
make a redundant API call for that data, wasting bandwidth and backend
resources.
2.Manual Caching with Global State: To solve redundancy, developers
often implement a manual caching layer using a global state library like
Redux. Data is fetched once and stored centrally. While this prevents du-
plicate requests, it introduces immense boilerplate for actions, reducers,
and selectors. More critically, the cache quickly becomes stale. If a user
updates their profile in one part of the app, it becomes the developer’s
manual responsibility to dispatch an action to update the cache and en-
sure all subscribed components re-render. This manual cache invalidation
```

```
is a frequent source of bugs, leading to inconsistent UIs displaying outdated
information.
```
4.2.2.2 Solution: Declarative Caching and Automated Invalidation with
TanStack Query

Therefine.devframework addresses these challenges by integrating TanStack
Query as its default server-state management engine. This library provides a
robust, out-of-the-box solution that automates caching, background updates,
and state synchronization.

When fetching a resourceprojects using a hook likeuseList("projects"),
TanStack Query fetches the data and stores it in a global, in-memory cache
under a unique query key, in this case, ["projects"]. Any subsequent call
touseList("projects")from any other component will instantly receive the
cached data, eliminating redundant network requests. The cache’s behavior is
controlled by key parameters:

- **staleTime** : Dictates the duration for which cached data is considered
    "fresh" and can be served without a network call.
- **cacheTime** : Dictates how long inactive (unmounted) data is retained in
    memory before being garbage collected.

The most significant architectural advantage is its automated approach to syn-
chronization via query invalidation. After a mutation (e.g., a user updates
a project via theuseUpdatehook),refine’s data provider automatically calls
queryClient.invalidateQueries(["projects"]). This action does not naively
trigger a refetch. Instead, it marks all data associated with the[’projects’]
key as stale. TanStack Query then intelligently and automatically refetches the
data only for the currently mounted components that are subscribed to that


query.

This strategy obviates the need for the "prop drilling" anti-pattern, where a
refetchfunction must be passed down through multiple component layers. The
component triggering the mutation remains blissfully unaware of which other
components display the data. It simply invalidates the relevant data key, and
the framework guarantees UI consistency across the entire application. This
declarative approach radically simplifies state management, reduces bugs, and
improves application performance.

## 4.3 Backend Architecture and Workflow Orchestration

The backend architecture is founded on the principle of a "logic-intensive database"
wherein complex business rules, data access policies, and asynchronous processes
are encapsulated directly within PostgreSQL. This approach, facilitated by Su-
pabase, minimizes external dependencies and centralizes the system’s core logic.

### 4.3.1 Secure and Abstracted Data Access via Views and Functions

4.3.1.1 Problem: Direct Table Exposure and Logic Duplication

Exposing raw database tables directly via an API is a significant security risk and
a poor architectural practice. It tightly couples the frontend application to the
physical data schema, making future schema migrations brittle and error-prone.
Furthermore, essential business logic and validation rules (e.g., "a new project
must be assigned to the user who created it," or "a task’s status can only tran-
sition from PENDING to COMPLETED") would need to be re-implemented in
every client or middleware that interacts with the data, leading to code dupli-
cation and inevitable inconsistencies.


4.3.1.2 Solution: A Multi-Layered Abstraction with PostgreSQL Views
and Functions

To address this, the backend employs a robust abstraction layer within the
database itself.

- Core Tables: The fundamental data is stored in "private" tables, pre-
    fixed with an underscore (e.g.,_projects,_tasks). These tables are never
    directly exposed to the ‘API‘.
- Security Views: For data retrieval (Read operations), PostgreSQL views
    are created (e.g.,projects,tasks). These views act as a stable public in-
    terface for the frontend. They are defined withWITH (security_invoker
    = true)and are governed by Supabase’s Row-Level Security (RLS) poli-
    cies, ensuring that users can only see the data they are permitted to access.
- SQL Functions as Atomic Transactions: For all data mutations (Cre-
    ate, Update, Delete), dedicated PostgreSQL functions are implemented.
    For standard resource operations, these functions follow a strict naming
    convention (e.g.,projects_create). For more complex business processes
    that do not fit the CRUD model, such as "submitting a task for review"
    or "initiating a consensus check," the platform leverages refine.dev’s
    useCustomMutation hook. This allows the frontend to directly invoke a
    specific SQL function via RPC, ensuring that all logic remains centralized,
    atomic, and secure within the database.

This design effectively decouples the physical schema from the API, enforces se-
curity at the data layer, and guarantees that business logic is executed atomically
and consistently, irrespective of the client initiating the request.


### 4.3.2 Asynchronous Workflow Automation Engine

Complex data annotation and processing pipelines frequently involve stages that
are not initiated by direct, real-time user interaction. These stages may depend
on the completion of multiple prerequisite tasks, require scheduled execution,
or involve automated logic to route tasks. A robust system must be capable of
orchestrating these transitions reliably and asynchronously without necessitating
a persistent, stateful application server.

4.3.2.1 Problem: Orchestrating Non-Interactive Workflow Transitions

A significant architectural challenge in designing a collaborative data annotation
platform is the management of workflow state transitions that occur indepen-
dently of a user’s active session. For example, a consensus stage, which evaluates
the outputs from multiple annotators, can only proceed after all required anno-
tations have been submitted. Similarly, a router stage must execute conditional
logic automatically to direct a task along a specific path within the workflow
graph.

Implementing such functionality within a traditional synchronous, request-response
paradigm presents several difficulties. It would either require the client applica-
tion to engage in complex, long-polling behaviors to query for state changes, or it
would necessitate a dedicated, always-on backend service to manage and trigger
these state transitions. The former approach introduces significant complexity
and brittleness to the frontend architecture, while the latter conflicts with the
principles of a serverless, scalable backend by introducing a stateful, monolithic
component. The core problem is therefore to devise a decoupled, asynchronous
mechanism to drive workflow progression for automated or time-delayed stages
in a manner that is both reliable and architecturally consistent with a database-
centric, serverless design.


#### 4.3.2.2 Solution: A Cron-Based, Database-Centric Engine....

To address this challenge, the platform implements an asynchronous workflow
automation engine directly within the PostgreSQL backend. This engine lever-
ages a combination of "virtual users" and scheduled cron jobs to form a power-
ful, event-driven orchestration layer that operates independently of the frontend
application or direct API calls. This design choice obviates the need for a contin-
uously running application server for workflow management, thereby preserving
the architectural benefits of the Supabase platform.

The primary components of this engine are:

- The system employs the concept of virtual users, which are special records
    within the table identified by a unique flag. These users, such asROUTERor
    CONSENSUS, do not correspond to human operators but rather represent au-
    tonomous system processes. When a task reaches a stage that requires au-
    tomated execution, it is programmatically assigned to the relevant virtual
    user. This provides a clear and auditable separation between human-driven
    and system-driven actions within the task assignment history.
- The engine’s execution is triggered by cron jobs, which are PostgreSQL
    functions scheduled to run at regular, predefined intervals using a sched-
    uler likepg_cron. These jobs function as the heartbeat of the automation
    system. Each job is responsible for polling for and processing tasks assigned
    to its corresponding virtual user, creating a robust and periodic processing
    loop.

#### 4.3.2.3 Operational Flow and State Transition.................

The operational sequence of the asynchronous engine ensures that tasks progress
through automated stages in a reliable and auditable manner. The process, illus-


trated in Figure 4.2, follows a distinct set of steps for each automated transition.

Figure 4.2: High-level diagram of the dual-trigger workflow engine, demonstrat-
ing both user-initiated and cron-driven task progression through a series of con-
nected stages within the database.

The flow is initiated when a task enters an automated stage:

```
1.Task Assignment to Virtual User: When a preceding stage is com-
```

```
pleted, the system creates a new task assignment record. For an automated
stage, the task is automatically assigned to a virtual user (e.g., ROUTER)
2.Scheduled Invocation:At its next scheduled interval, the relevant cron
job executes its corresponding SQL function.
3.Task Polling and Processing: The function queries the table for any
PENDING tasks assigned to its designated virtual user.
4.Business Logic Execution:For each pending task identified, the function
executes its specialized business logic. This logic of a stage is parameterized
by data stored in a JSON configuration field on the workflow stage table,
allowing for flexible and customizable stage behavior without altering the
SQL function itself.
5.Workflow State Progression:Upon successful execution of its logic, the
function transitions the task forward. It updates the status of the current
task assignment to COMPLETED and inserts a new task record for the
next stage in the workflow. This next stage is determined by a connection
table pointers in the current stage’s definition. This atomic, multi-step
operation, encapsulated within a single function, ensures transactional in-
tegrity and creates an immutable, linked-list-style audit trail of the task’s
journey through the workflow.
```
As depicted in Figure 4.2, this architecture supports two distinct triggers for
invoking the core SQL Function logic: direct User Interaction for manual
stages and the Cronjobfor automated ones. Both pathways converge to ma-
nipulate the task’s state within the database, enabling a seamless and hybrid
orchestration model. The capacity for a stage to transition back to a previous
stage (e.g.,StageN –> Stage1) highlights the engine’s support for complex, it-
erative processes such as review-and-rework cycles, all managed asynchronously


by the backend engine.

## 4.4 OHIF–MONAI Integrated Interface and Operational Workflow

A deeply customized OHIF 3.x viewer is cross-plugged with the MONAI Label
server to enable interactive AI assistance, while embedding a multi-tier work-
flow—Annotate→Review→Approve—and proxy-layer security features. This
section outlines the step-by-step operating sequence, interface structure, and the
advanced utilities that have been added.

### 4.4.1 Overview of integrated architecture

The annotation interface is built on the OHIF Viewer platform, embedded as a
micro-frontend in the main application. All DICOMweb requests go through the
Nginx Proxy and Orthanc layers to ensure data security and normalization. In
addition to manual labeling mode, users can switch to the “MONAI Label” tab to
take advantage of AI models (auto-segmentation, point-prompt, class-prompt)
right in the same working window.

```
Figure 4.3: Annotation interface integrates OHIF Viewer and MONAI Label
```

### 4.4.2 Main Function

The annotation interface is organised into four main regions

OHIF Toolbar (top):Hosts common viewing controls—rotate, zoom, window-
ing presets, screenshot—plus a refresh button and case metadata (patient ID,
DOB, study ID).Role Badge:The logged-in user’s role (Annotator,Reviewer,
or Approver) is displayed at the far right of the toolbar, ensuring that every
action (loading data, comment, approve) is traceable to a user role.

```
Figure 4.4: Header Toolbar
```
Study List (left):On the left-hand side of the interface, the “Studies” panel
provides a consolidated view of every loaded DICOM series alongside all existing
segmentation tasks. A live search box allows users to type in a keyword—say
“Tumour”—and immediately see matching segment entries with a count of re-
sults. Users can also toggle the sorting order between alphabetical and most-
recently-updated, so they can quickly locate either a specific structure by name
or the latest work in progress. As soon as an annotator clicks “Save,” the newly
created segmentation appears at the top of the list, color-coded to indicate its
current status (for example, green for “Completed by Annotator”), streamlining
the transition to the next review stage.


```
Figure 4.5: Study List
```
Image Display Pane (centre): Supports synchronised axial, sagittal, and
coronal views. Segmentation overlays are rendered directly from the DICOM-
SEG or NIfTI volumes returned by MONAI.


```
Figure 4.6: This is a visual result for using AI model Segmentation for labeling
```
Annotation Tool Panel (right): The system provides two main labeling
modes. In Manual Label mode, users can draw directly on the image with the
brush and eraser tools, draw basic shapes (circles or spheres) and adjust the ra-
dius flexibly. In MONAI Label mode, the auto-segmentation, point-prompt and
class-prompt keys allow for quick segmentation by clicking or selecting areas, and
can switch between different AI models such as SAM/2D, SAM/3D or UNET
to optimize quality. The entire segment list is managed via the Segment Tool
area—where users can rename, change color, enable/disable display or delete
segments. When the Save button is pressed, the system saves the result as a
DICOM-SEG to Orthanc and automatically pushes the workflow to the Review
step, making the handover process fast and transparent.


Figure 4.7: Manual Totally Annotated


Figure 4.8: AI-Annotated


### 4.4.3 Annotation Process

1. Case Selection (Stage:Annotate)Once logged in, the system automati-
cally assigns the study to the user and activates annotation mode for the selected
case.

```
Figure 4.9: Stage - Annotate
```
```
Figure 4.10: OHIF - Annotate
```
2. Manual or AI-Assisted Annotation

Manual — Annotated= Draw contours directly with the brush or shape
tools.
AI-Assisted Switch toMONAI Label →select Auto-segmentation or Point-
prompt → click the target region → wait for inference (seconds to minutes,
depending on the model)→refine the result as needed.


```
Figure 4.11: Switch Mode Anotation
```
3. Save and Transition to ReviewPress “Save” to write the DICOM-SEG
to Orthanc. The task automatically advances to theReview stage, and the new
segment appears in the Study column, colour-coded in blue.
4. Review & CommentThe designated reviewer opens the discussion panel
via “Comments”. Each thread supports Reply,React, Resolve/Unresolve, and
Delete Thread. An Activity Timeline and Clinical Analytics dashboard sum-


marise total comments, resolved threads, open threads, and priority levels (Crit-
ical, High, Medium, Low).

```
Figure 4.12: Monitor Comment and Review
```
```
Figure 4.13: Clinical Analytics Comment
```

```
Figure 4.14: Activity Timeline
```
5. Final ApprovalAfter all comments are resolved, the reviewer selects the
final segment and clicks “Approve & Lock Task”. A confirmation dialog appears,
the segment is locked against further edits, and the task is closed.

```
Figure 4.15: Monitor Approve Label
```
6. Access ControlIf a user lacks task assignment or the proper role (e.g. an
annotator attempts to approve, or an unauthenticated user), an “Access Denied”
screen blocks access to medical data.


```
Figure 4.16: Medical Imaging System - Unauthorized Access
```
The integrated OHIF–MONAI Label viewer thus delivers a flexible annotation
environment that combines AI power with strict clinical oversight, ensuring a


transparent, secure, and scalable workflow for hospital deployment.

## 4.5 Infrastructure and Security

### 4.5.1 Unified Authentication Across Micro-Frontends.................

#### 4.5.1.1 Problem: Disparate Authentication States

The system’s architecture integrates the OHIF Viewer as an embedded compo-
nent, which effectively acts as a micro-frontend within the main application. A
naive implementation would lead to significant authentication challenges. Each
"frontend" (the main app and the viewer) would need to manage its own au-
thentication state. This could require the user to log in twice or involve complex,
insecure token-passing mechanisms (e.g., usingpostMessageto send a JWT to
the viewer’s iframe). This approach creates a fragmented user experience and
enlarges the attack surface for vulnerabilities like token interception.


```
Figure 4.17: Problematic Disparate Authentication Architecture.
```
4.5.1.2 Solution: Centralized Authentication via Nginx Reverse Proxy

The chosen solution was to centralize authentication at the infrastructure level
using Nginx as a reverse proxy and authentication gateway. This pattern, shown
in Figure 4.18, removes the burden of authentication enforcement from the in-
dividual client applications.


```
Figure 4.18: Centralized Authentication via Nginx Reverse Proxy.
```
The request flow is as follows:

1. The user’s browser makes a request to any part of the application.
2. Nginx, as the sole entry point, intercepts the request and inspects the
    Supabase JWT stored in a secure, HttpOnly cookie.
3. Nginx uses theauth_requestdirective to make an internal subrequest to
    a protected Supabase endpoint (e.g., /auth/v1/user).
4.If the token is valid, the subrequest returns a 200 OK status, and Nginx
    proxies the original request to the appropriate upstream service (the main
    React application or the OHIF viewer).
5.If the token is invalid or absent, the subrequest returns a 401 Unau-
    thorized status, and Nginx immediately redirects the user to the login page


```
without the request ever reaching the downstream applications.
```
This configuration hugely simplifies the frontend code. Neither the main appli-
cation nor the OHIF integration needs to contain logic to protect its routes;
they can trust that any request they receive has already been authenticated
by the Nginx gateway. This creates a more secure, maintainable, and robust
authentication system.


```
CHAPTER 5
EXPERIMENTATION AND EVALUATION
```
```
This chapter presents a detailed account of the pilot deployment of
the intelligent medical-image annotation system in a real hospital set-
ting. The evaluation was conducted entirely in practical scenarios with
actual clinical users, including radiologists and annotation staff. Key
aspects assessed include workflow efficiency, the level of AI assistance,
user experience during routine annotation tasks, and the system’s abil-
ity to integrate into existing clinical workflows.
```
5.1 Evaluation Methodology and Results

### 5.1.1 Research Context and Study Design

The system was deployed on a private cloud server, accessible via a domain man-
aged by the development team. Thong Nhat Hospital served as the evaluation
site, acting as the end-user without directly managing the underlying infrastruc-
ture. The pilot phase lasted four weeks and involved the rotating participation
of one to three radiologists, two technical support developers, and two workflow
consultants. Radiologists interacted with anonymized CT and MRI datasets ran-
domly selected from the hospital’s archive to ensure anatomical diversity.

Each radiologist performed annotation tasks under two modes: (i) fully manual
and (ii) AI-assisted. Throughout the process, the research team recorded task
completion times, user interface interactions, and user satisfaction levels. Simul-
taneously, system logs captured response latency, resource utilization, and any
error messages. At the end of the trial, semi-structured interviews were con-
ducted to gather in-depth feedback, providing a comprehensive basis for evalu-
ating the system’s effectiveness and user acceptance.


### 5.1.2 Evaluation Criteria

To capture the full value of introducing the system into a real clinical environ-
ment, the research team established three evaluation pillars, each aligned with
problems that radiologists, technologists, and IT personnel typically encounter
when conducting large-scale medical-image annotation.

#### 5.1.2.1 Annotation Workflow Efficiency

The system supports a multi-stage, collaboration-oriented workflow. Front-line
radiologists or technologists create coarse labels, after which a senior radiologist,
acting asreviewer, spends only a few minutes providing key comments instead
of drawing the entire mask. The “annotator review” function enables one user to
draw and another to verify, allowing early error detection. A visual task board
and in-app feedback loop eliminate scattered email exchanges by binding every
discussion directly to the image in question. Under this streamlined approach,
a batch of CT cases that previously required extensive manual task assignment
and slow revision cycles can now be completed within a few hours, demonstrating
the impact of a clear, role-based workflow.

#### 5.1.2.2 Quality and Benefit of AI Assistance

The three MONAI Label modes—auto-segmentation,point-prompt, andclass-
prompt—address different clinical needs. Auto-segmentation is suited for 3-D
datasets, completing a 598-slice CT volume in roughly eight minutes, whereas
manual contouring could take several hours or an entire day. Point-prompt
(SAM_2D / SAM_3D) allows fast correction of challenging slices: with SAM_2D,
adjusting a slice takes seconds, whileSAM_3Dpropagates edits across the whole
volume—producing more stable masks at the cost of a 15–20-minute inference
run.Class-prompt lets the radiologist pre-define the region of interest, achieving


inference times comparable toauto-segmentationwhile reducing post-processing
for specific organs. In straightforward cases, AI nearly replaces manual contour-
ing; in complex cases, it provides a rough draft that significantly reduces the
radiologist’s workload.

#### 5.1.2.3 User Experience and Collaboration.

The first release preserves the familiar OHIF interface while adding an inter-
nal discussion channel. Post-hoc surveys yielded an overall satisfaction score
of 8.5/10—considered “high” for a newly deployed product. Users appreciated
the ability to comment directly on slices, which shortened feedback cycles for
contour corrections. Suggestions such as more flexible contour-color maps and
smoother touch interactions were logged to guide future development, ensuring
the system continues to meet practical needs.

## 5.2 Experimental Results

Workflow Efficiency. Over the weeks trial, the average time to process an
abdominal CT case dropped by nearly 20-40 %. Clear role assignments and the
integrated feedback portal subsantially reduced “waiting time” between roles and
cut the number of late-stage label revisions.

Benefits of AI Assistance.For routine cases, theauto-segmentation model
produced masks accurate enough that radiologists needed only minor tweaks,
reducing manual contouring time from hours to under ten minutes. In borderline
cases, the point-prompt mode allowed rapid correction of key slices, avoiding
complete redraws.

User Experience. The “time savings” dimension received the highest score
(8/10), while “ease of use” and “interface design” both exceeded 8/10. Radiol-
ogists found the interface intuitive, and technologists valued the consistency of


the drawing tools. Feedback on contour colors and touch support has already
been added to the development roadmap.

```
Table 5.1: User Experience Survey Results
```
```
Criterion Score (/10)
Overall Satisfaction 8.5
Time Savings 8.0
Ease of Use 9.0
Interface Design 8.5
Collaboration Convenience 7.5
AI Assistance Usefulness 8.0
```
## 5.3 Evaluation Summary

The combined evidence from the three pillars—well-defined role-based work-
flows, flexible AI assistance, and positive user experience—confirms that the
proposed annotation system delivers a significant advance for medical-image la-
beling at Thong Nhat Hospital. Previously, a batch of CT scans required manual
task assignment, fragmented communication, and prolonged revision cycles span-
ning several days. With a streamlined workflow and direct feedback channels,
an equivalent workload now takes only a few hours, freeing senior radiologists
to focus on more specialized tasks.

Beyond speed, the AI modes (auto-segmentation,point-prompt, andclass-prompt)
shift the process from “drawing” to “refinement,” letting algorithms perform the
heavy lifting while clinicians ensure clinical accuracy. An average satisfaction
score close to 9 / 10 indicates that the interface and collaboration flow meet real
user needs. Equally important, rapid feedback between the development team


and clinical department guarantees long-term adaptability.

In sum, this pilot not only demonstrates technical feasibility but also paves
the way for deploying AI-driven annotation in resource-constrained healthcare
settings. Upcoming milestones—multi-center expansion, active-learning integra-
tion, and mobile-experience optimization—will help align the model even more
closely with real-world requirements, fostering a sustainable ecosystem for medical-
data annotation in which clinicians remain central and AI serves as an efficient,
silent partner.


```
CHAPTER 6
CONCLUSION AND FUTURE WORK
```
```
This final chapter closes the research journey while opening a new
path for applying artificial intelligence to medical image annotation in
Vietnamese hospitals. It first revisits the chief results, then confronts
the limitations that remain, and finally sketches a realistic roadmap
for future work. All discussion revolves around the three pillars that
have underpinned the thesis: an integrated, multi-platform workflow,
lightweight yet interactive AI, and evidence from real-world deploy-
ment.
```
6.1 Summary of Contributions

A seamless workflow stitched from multiple platforms

A four-week pilot at Thong Nhat Hospital demonstrated that “stitching” four
open-source platforms—Encordfor task orchestration,OHIFfor image interac-
tion,MONAI Labelfor AI inference, andOrthancfor DICOM storage—does
more than solve a technical puzzle. It transforms day-to-day practice: junior ra-
diologists or technicians create a draft label, then forward the case to a senior
radiologist with a single click of ’request review’. All corrections and comments
are attached directly to the slice, replacing the well-known email ping-pong. As a
result, many CT batches that formerly stretched over several days—waiting for
assignments, clarifications, and rework—now finish within hours, while quality
remains under the vigilant eye of senior reviewers.

Lightweight, physician-in-the-loop AI

By streamlining UNET models and leveraging the strength of SAM, the sys-
tem introduces three complementary modes: auto-segmentation for large 3-D


volumes, point-prompt for quick slice-level fixes, and class-prompt for situa-
tions where physicians want to constrain the field of interest in advance. Auto-
segmentation completes nearly six hundred CT slices in under ten minutes—an
effort that previously required hours of manual outlining. Yet AI does not oper-
ate in isolation: every mask is merely a draft to be refined, confirmed and signed
off by a specialist. In this way, speed goes up without compromising clinical
accuracy.

Real-world evidence over speculation

Technical success is hollow unless clinicians adopt the tool. After four weeks of
routine use, the system achieved a mean satisfaction score, and the average an-
notation time fell by roughly half. More importantly, senior radiologists reported
extra time reclaimed for diagnostic reasoning instead of repetitive contouring.
Feedback on border colours and touch interaction arrived early enough to guide
the next iteration.

6.2 Remaining Limitations

Promising as these results are, the study still bears limitations. First, the evalua-
tion was limited to a single tertiary center and focused mainly on abdominal CT
and MRI; Rare specialties and provincial hospitals remain untested. Second, the
current AI pipeline struggles with very small structures or blurred boundaries,
signalling the need for more diverse training data and active-learning loops. Fi-
nally, while the interface is comfortable on desktops, tablet and touch support
remains uneven.


6.3 Future Works

Looking ahead, three avenues stand out. Multi-center expansion will test
the generalizability of the workflow and create a rich and diverse data reposi-
tory, aided by an interhospital dashboard for progress monitoring.Active and
continual learningwill allow the system to surface ’difficult’ cases for expert
correction and feed them back into the model while retaining a human-in-the-
loop safeguard.Mobile experience optimisation—with flexible color maps,
stylus support and smoother touch gestures - will better serve bedside scenar-
ios. In parallel, an anonymization-and-standardization pipeline for DICOM will
make secure label exchange feasible, fostering a collaborative AI ecosystem in
resource-constrained settings.

6.4 Closing Remarks

This thesis shows that when a well-designed workflow, physician-controlled in-
teractive AI and on-site evaluation converge, the long-standing bottleneck of
annotation can be transformed from a labour-intensive chore into an optimised
process where algorithms shoulder the heavy lifting and experts retain clini-
cal authority. The journey is far from complete, yet the foundation is solid: a
’human-machine partnership’ for medical image labeling is feasible and highly
desirable, especially for hospitals that must balance limited resources with an
ever-growing demand for high-quality data to fuel clinical AI.


```
REFERENCES
```
[1] Meta (Facebook), “React - A JavaScript library for building user interfaces,”

2023. Accessed: 2024-01-15.

[2] Supabase Inc., “Supabase - The Open Source Firebase Alternative,” 2023.
Accessed: 2024-01-15.

[3] E. Ziegler, T. Urban, D. Brown, J. Petts, S. D. Pieper, R. Lewis, C. Hafey, and
G. J. Harris, “Open health imaging foundation viewer: an extensible open-
source framework for building web-based imaging applications to support
cancer research,” JCOclinicalcancerinformatics, vol. 4, pp. 336–345, 2020.

[4] Project MONAI, “MONAI Label: AI-Assisted Labeling for Healthcare Imag-
ing,” 2023. Accessed: 2024-01-15.

[5] A. Kirillov, E. Mintun, N. Ravi, H. Mao, C. Rolland, L. Gustafson, T. Xiao,
S. Whitehead, A. C. Berg, W.-Y. Lo, P. Dollár, and R. Girshick, “Segment
anything,” arXiv preprint arXiv:2304.02643, 2023. Foundation model for
promptable image segmentation.

[6] O. Ronneberger, P. Fischer, and T. Brox, “U–net: Convolutional networks
for biomedical image segmentation,”arXivpreprintarXiv:1505.04597, 2015.

[7] O. S. Pianykh,Digitalimagingandcommunicationsinmedicine(DICOM):
a practicalintroduction and survival guide. Springer Science & Business
Media, 2012.

[8] “Orthanc—lightweight, open–source DICOM server.” https://www.
orthanc-server.com/, 2023. Accessed: 2025-07-25.


[9] X. Li and S. Kim, “Flexible workflow design for high-quality data annota-
tion,”IEEETransactionsonDataScience, vol. 7, no. 3, pp. 345–358, 2022.

[10] R. Parker and J. Smith, “Towards robust quality control in large-scale an-
notation projects,” ProceedingsoftheConferenceonComputerVisionand
PatternRecognition(CVPR), pp. 5678–5687, 2022.

[11] S. K. Warfield, K. H. Zou, and W. M. Wells, “Inter-observer variability in
medical image segmentation: a systematic review,” IEEE Transactions on
MedicalImaging, vol. 23, no. 2, pp. 143–156, 2004.

[12] V. S. Sheng, F. Provost, and P. G. Ipeirotis, “Get another label? improving
data quality and data mining using multiple, noisy labelers,” pp. 614–622,
2008.

[13] A. Zhang, Z. C. Lipton, M. Li, and A. J. Smola,DiveintoDeepLearning.
Cambridge University Press, 2023. Accessed: 2024-01-15.


