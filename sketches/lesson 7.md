% ====================================================================
% A/L ICT - Lesson 7: Systems Analysis & Design Cheat Sheet
% Optimized for A4 B&W Printing using LaTeX
% Designed for use on Overleaf.com
% ====================================================================

% --- Document Class & Packages ---
\documentclass[a4paper, 8pt]{extarticle}

% --- Geometry for Margins ---
\usepackage[a4paper, margin=1cm, top=1.2cm, bottom=1.2cm]{geometry}

% --- Essential Packages ---
\usepackage{multicol}        % For creating multi-column layouts
\usepackage[svgnames]{xcolor} % For colors (we'll use shades of gray)
\usepackage{tcolorbox}       % For creating styled boxes
\usepackage{enumitem}        % For customizing lists
\usepackage{graphicx}        % To scale images/symbols if needed

% --- Font Setup (for a clean, modern look) ---
\usepackage{fontspec}
\setmainfont{Inter}
\setmonofont{Roboto Mono}

% --- Custom Commands for Styling ---
\newcommand{\sectionheading}[1]{\large\textbf{#1}\par\noindent\rule{\linewidth}{0.4pt}}
\newcommand{\subsectionheading}[1]{\normalsize\textbf{#1}}
\tcbset{
  colback=gray!10, colframe=gray!75, boxrule=0.5pt,
  sharp corners, boxsep=4pt, left=4pt, right=4pt, top=4pt, bottom=4pt
}
\setlist[itemize]{leftmargin=*, noitemsep, topsep=3pt, label=\textbullet}

% --- Start of the Document ---
\begin{document}
\pagestyle{empty} % Removes page numbers

% --- Title ---
\begin{center}
    \fontsize{12pt}{14pt}\selectfont
    \textbf{Lesson 7: Systems Analysis \& Design}
\end{center}
\vspace{1em}

% --- Main 2-Column Layout ---
\begin{multicols}{2}

% =============================================
% --- COLUMN 1 ---
% =============================================

\sectionheading{1. Foundation: Concepts \& Models}
\vspace{0.5em}
\subsectionheading{System Concepts}
\begin{itemize}
    \item \textbf{Definition:} Interrelated components working together to achieve an objective.
    \item \textbf{Classifications:} Open vs. Closed; Natural vs. Man-made; Living vs. Physical.
\end{itemize}

\subsectionheading{Types of Information Systems}
\begin{itemize}
    \item \textbf{TPS:} For \textit{Operational Level} (daily routine transactions).
    \item \textbf{MIS:} For \textit{Management Level} (routine summary reports).
    \item \textbf{DSS:} For \textit{Management Level} (semi-structured decisions).
    \item \textbf{ESS:} For \textit{Strategic Level} (unstructured decisions).
    \item \textbf{OAS:} Increases office worker productivity.
    \item \textbf{KMS:} Manages organizational knowledge.
    \item \textbf{ERP:} Integrates all business functions.
    \item \textbf{Expert System:} AI-based, mimics a human expert.
\end{itemize}

\subsectionheading{SDLC Models & Applicability}
\begin{itemize}
    \item \textbf{Waterfall:} Sequential. \textit{Best for stable requirements.}
    \item \textbf{Spiral:} Iterative + Risk Analysis. \textit{Best for large, high-risk projects.}
    \item \textbf{Agile:} Iterative, rapid delivery. \textit{Best for changing requirements.}
    \item \textbf{Prototyping:} Build a working model for early feedback.
    \item \textbf{RAD:} Develop modules in parallel for fast delivery.
\end{itemize}

\subsectionheading{Development Methodologies}
\begin{itemize}
    \item \textbf{Structured:} Traditional, top-down (e.g., SSADM).
    \item \textbf{Object-Oriented:} Models system as interacting objects.
\end{itemize}

\vspace{1em}
\sectionheading{2. Beginning: Planning \& Analysis}
\vspace{0.5em}
\subsectionheading{Feasibility Study (Is it possible?)}
\begin{itemize}
    \item \textbf{T}echnical: Do we have the tech/skills?
    \item \textbf{E}conomic: Do benefits justify cost?
    \item \textbf{O}perational: Will people use it?
    \item \textbf{O}rganizational: Does it support company goals?
\end{itemize}
\subsectionheading{Requirement Analysis (What should it do?)}
\begin{itemize}
    \item \textbf{Functional:} The \textit{activities} it must perform.
    \item \textbf{Non-functional:} The \textit{qualities} or constraints (e.g., speed, security).
    \item \textbf{IEEE Standard:} Essential needs use ``Shall''; desirable ones use ``Should''.
\end{itemize}

\columnbreak % End Column 1, Start Column 2

% =============================================
% --- COLUMN 2 ---
% =============================================

\sectionheading{3. Middle: Design \& Testing}
\vspace{0.5em}
\subsectionheading{Analysis & Modeling Tools}
\begin{itemize}
    \item \textbf{DFD (Data Flow Diagram):} Shows data movement.
    \begin{itemize}
        \item \textit{Components:} External Entity, Process, Data Flow, Data Store.
        \item \textit{Levels:} Context Diagram (Level 0), Level 1 DFD.
    \end{itemize}
    \item \textbf{LDM (Logical Data Modeling):} Shows data structure.
    \begin{itemize}
        \item \textit{Components:} Entity, Attribute, Relationship.
        \item \textit{Cardinality:} One-to-One, One-to-Many, etc.
    \end{itemize}
    \item \textbf{Other Terms:} SSADM, EPD, BSO.
\end{itemize}

\subsectionheading{System Design}
\begin{itemize}
    \item \textbf{Logical Design:} What the system must do (tech-independent).
    \item \textbf{Physical Design:} How it will be implemented (with tech).
    \item \textbf{Database Mapping:} Entity $\rightarrow$ Table, Attribute $\rightarrow$ Field.
    \item \textbf{Data Dictionary:} A repository of metadata (data about data).
\end{itemize}

\subsectionheading{System Testing (Does it work?)}
\begin{tcolorbox}[title=\textbf{Testing Techniques & Levels}]
    \begin{itemize}
        \item \textbf{White-box:} Tests internal code structure.
        \item \textbf{Black-box:} Tests functionality without seeing code.
    \end{itemize}
    \vspace{0.5em}
    \textit{Testing Levels (Bottom-up):}
    \begin{enumerate}
        \item \textbf{Unit Testing} (by programmers).
        \item \textbf{Integration Testing}.
        \item \textbf{System Testing} (by a separate test team).
        \item \textbf{Acceptance Testing} (by users).
    \end{enumerate}
\end{tcolorbox}

\vspace{1em}
\sectionheading{4. End Game: Deployment \& Alternatives}
\vspace{0.5em}
\subsectionheading{Deployment / Changeover Methods}
\begin{itemize}
    \item \textbf{Parallel:} Old \& New run together. \textit{Safest, most expensive.}
    \item \textbf{Direct (Big Bang):} Stop Old, start New. \textit{Riskiest, cheapest.}
    \item \textbf{Phased:} Implement New system in parts.
    \item \textbf{Pilot:} Implement for a small group first.
\end{itemize}
\subsectionheading{COTS vs. Custom Software}
\begin{itemize}
    \item \textbf{COTS (Commercial-Off-The-Shelf):} Buying a package.
    \begin{itemize}
        \item \textit{Pros:} Cheaper, faster.
        \item \textit{Cons:} May not fit perfectly, no competitive advantage.
    \end{itemize}
    \item \textbf{Custom Developed:} Building from scratch.
    \begin{itemize}
        \item \textit{Pros:} Perfect fit, competitive advantage, becomes an asset.
        \item \textit{Cons:} Expensive, time-consuming.
    \end{itemize}
    \item \textbf{Key Concepts:} Gap Analysis, Business Process Reengineering.
\end{itemize}

\end{multicols}
\end{document}
