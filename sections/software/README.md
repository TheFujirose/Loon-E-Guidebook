# Software Section of Loon-E Guidebook
Please update this document when adding new sections

Entry point is `overview.tex`, which should provide an overview of the software architecture and design. 

The files are organized to first overview the two main software components: the basestation and the GUI. Then, the basestation is further broken down into the primary computer and development information for the software team.

> ![IMPORTANT] 
> Keep highest level of section to `\subsection` to maintain consistency and readability. Use `\subsubsection` for more detailed breakdowns within sections, but avoid going deeper than that to prevent clutter and maintain a clear structure in the document.

File Hierarchy:
```bash
software/
├── README.md
├── basestation/
│   ├── primary/                    # Covers the development information for the Jetson Orin
│   ├── development/                # Covers the basestation information for the software team
│   │    ├── development.tex        # Covers the basestation information for the software team
│   │    └── specifications.tex     # Covers the basestation information for the software team
│   ├── basestation.tex             # Covers the basestation for non-technical and technical audiences
│   └── gui.tex                     # Coveres the GUI for non-technical and technical audiences
└── overview.tex                    # Covers the overview of the software architecture and design
```