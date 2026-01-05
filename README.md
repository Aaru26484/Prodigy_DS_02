\documentclass[11pt]{article}

\usepackage[a4paper,margin=1in]{geometry}
\usepackage{hyperref}
\usepackage{graphicx}
\usepackage{enumitem}
\usepackage{xcolor}

\title{\textbf{Prodigy Infotech -- Data Science Internship}\\
Task 02: Data Cleaning \& Exploratory Data Analysis (EDA)}
\author{\textbf{Aarti Singh}}
\date{}

\begin{document}
\maketitle

\section*{Task Overview}
This task focuses on performing \textbf{data cleaning} and \textbf{exploratory data analysis (EDA)}
to understand the dataset, identify patterns, and explore relationships between variables.
EDA is a crucial step before applying any machine learning models.

\section*{Objectives}
\begin{itemize}[leftmargin=*]
    \item Clean and preprocess the dataset
    \item Handle missing and inconsistent values
    \item Analyze numerical features
    \item Identify correlations between variables
    \item Visualize insights using plots
\end{itemize}

\section*{Dataset}
\begin{itemize}[leftmargin=*]
    \item Dataset Used: Titanic Dataset
    \item Dataset contains passenger information such as age, fare, and survival status
\end{itemize}

\section*{Tools \& Technologies}
\begin{itemize}[leftmargin=*]
    \item Python
    \item Pandas
    \item NumPy
    \item Matplotlib
    \item Seaborn
    \item Google Colab / Jupyter Notebook
\end{itemize}

\section*{Exploratory Data Analysis}
The following steps were performed during EDA:
\begin{enumerate}[leftmargin=*]
    \item Data loading and inspection
    \item Handling missing values
    \item Selecting numerical features
    \item Computing correlation matrix
    \item Visualizing correlations using a heatmap
\end{enumerate}

\section*{Correlation Heatmap}
A correlation heatmap was generated to visualize relationships between numerical features in the dataset.
This helps in identifying strong positive and negative correlations and assists in feature selection.

\begin{verbatim}
plt.figure(figsize=(8,6))

numeric_df = df.select_dtypes(include=['int64', 'float64'])
sns.heatmap(numeric_df.corr(), annot=True, cmap='coolwarm')

plt.title("Correlation Heatmap (Numeric Features)")
plt.show()
\end{verbatim}

\section*{Key Learnings}
\begin{itemize}[leftmargin=*]
    \item Importance of data cleaning before analysis
    \item Understanding feature relationships through correlation
    \item Effective visualization techniques in EDA
    \item Practical exposure to real-world datasets
\end{itemize}

\section*{Acknowledgement}
I would like to thank \textbf{Prodigy Infotech} for providing this internship opportunity
and helping me enhance my data analysis and visualization skills.

\section*{Repository}
\href{https://github.com/}{GitHub Repository Link}

\end{document}
