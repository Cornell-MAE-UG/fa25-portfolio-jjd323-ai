---
layout: project
order: 1
title: Rocketry Project 2025-2026
description: Year long project focused on insulating and dust-proofing launch-critical ground station. 
technologies: [SolidWorks, 3D Printing]
image: /assets/images/CRT-Logo.png
---
<style>
\NeedsTeXFormat{LaTeX2e}
\ProvidesPackage{rocketry}[01/20/22 Cornell Rocketry Team]

\RequirePackage[utf8]{inputenc}

\RequirePackage[T1]{fontenc}
\RequirePackage{newpxtext,newpxmath} 
\RequirePackage{geometry}
\RequirePackage{hyperref}
\RequirePackage{changepage}
\RequirePackage{eso-pic}
\RequirePackage{graphicx}
\RequirePackage{tcolorbox}
\RequirePackage[T1]{fontenc}
\RequirePackage{enumitem}

\newlist{todolist}{itemize}{2}
\setlist[todolist]{label=$\square$}

\newcommand\subteam[1]{\renewcommand\@subteam{#1}}
\newcommand\@subteam{}

\geometry{margin=1in, tmargin=1in}
\hypersetup{
    pdftitle={Technical }, 
    pdfauthor={\@author},
    colorlinks=true,
    linkcolor=black,
    urlcolor=blue,
    citecolor=blue,
    breaklinks=true,
}
\definecolor{dkgreen}{rgb}{0,0.6,0}
\definecolor{gray}{rgb}{0.5,0.5,0.5}
\definecolor{mauve}{rgb}{0.58,0,0.82}
\definecolor{rocket}{rgb}{0.70196, 0.10588, 0.10588}

\newcommand\BackgroundPic{%
\put(0,0){%
\parbox[b][\paperheight]{\paperwidth}{%
\vfill
\centering
\includegraphics[width=\paperwidth,height=\paperheight,keepaspectratio]{Images/background.jpg}%
\vfill
}}}

\renewcommand{\maketitle}[1]{
    \@ifundefined{@title}{\PackageError{rocketry}{Title missing}{You must specify a title to create a title page.}}{}
    \@ifundefined{@author}{\PackageError{rocketry}{Author missing}{You must specify an author to create a title page.}}{}
    \@ifundefined{@subteam}{\PackageError{rocketry}{Subteam missing}{You must specify a subteam to create a title page.}}{}
    \begin{titlepage}
    \begin{adjustwidth}{-0.5in}{-0.5in}

    \AddToShipoutPicture*{\BackgroundPic}
    
    \fontsize{44}{28}\selectfont
    \textbf{#1}
    
    \noindent\makebox[\linewidth]{\color{rocket}\rule{\paperwidth}{10pt}}
    
    \fontsize{24}{30}\selectfont
    \noindent \@author
    
    \noindent Cornell Rocketry Team

    \noindent \@title

    \noindent \@subteam
    
    \vspace{1.5in}
    \fontsize{20}{22}\selectfont
    
    \noindent Cornell University \\
    \noindent Sibley School of Mechanical and Aerospace Engineering \\
    \noindent 124 Hoy Road \\
    \noindent Ithaca, NY 14850
    \vspace{1in}
    \end{adjustwidth}
    \end{titlepage}
}

\newcommand*{\TakeFourierOrnament}[1]{{%
\fontencoding{U}\fontfamily{futs}\selectfont\char#1}}
\newcommand*{\danger}{\TakeFourierOrnament{66}}

\newcommand{\unusedtest}{\begin{tcolorbox}[colframe=rocket,colback=white]{\color{rocket} \danger} Test type is not being used.\end{tcolorbox}}


\newcommand{\PASS}[0]{\colorbox{green}{PASS}}
\newcommand{\FAIL}[0]{\colorbox{red}{\textcolor{white}{FAIL}}}
</style>

\section{Technical Report}
\subsection{Images of Design}

\begin{figure}[H]
    \centering
    \caption{\textbf{Dust Cover Designs}}
    \begin{subfigure}[b]{0.3\textwidth}
        \centering
        \includegraphics[width=\textwidth]{DustCover1.png}
        \caption{Dust Cover 1}
    \end{subfigure}
    \hfill
    \begin{subfigure}[b]{0.3\textwidth}
        \centering
        \includegraphics[width=\textwidth]{DustCover2.png}
        \caption{Dust Cover 2}
    \end{subfigure}
    \hfill
    \begin{subfigure}[b]{0.3\textwidth}
        \centering
        \includegraphics[width=\textwidth]{DustCover3.png}
        \caption{Dust Cover 3}
    \end{subfigure}

\end{figure}

\begin{figure}[H]
    \centering
    \caption{\textbf{Board Mount Designs}}
    \begin{subfigure}[b]{0.3\textwidth}
        \centering
        \includegraphics[width=\textwidth]{PowerBoardMount.png}
        \caption{Power Board Mount}
    \end{subfigure}
    \hfill
    \begin{subfigure}[b]{0.3\textwidth}
        \centering
        \includegraphics[width=\textwidth]{SenseBoardMount.png}
        \caption{Sense Board Mount}
    \end{subfigure}
    \hfill
    \begin{subfigure}[b]{0.3\textwidth}
        \centering
        \includegraphics[width=\textwidth]{SKAM-HatMount.png}
        \caption{SKAM-Hat Mount}
    \end{subfigure}

    \vspace{0.5cm}

    \begin{subfigure}[b]{0.3\textwidth}
        \centering
        \includegraphics[width=\textwidth]{SKAMBoardMount.png}
        \caption{SKAM-Board Mount}
    \end{subfigure}
    \hfill
    \begin{subfigure}[b]{0.3\textwidth}
        \centering
        \includegraphics[width=\textwidth]{IgnitorBoardMount.png}
        \caption{Ignitor Board Mount}
    \end{subfigure}
    \hfill
    \begin{subfigure}[b]{0.3\textwidth}
        \centering
        \includegraphics[width=\textwidth]{BallValveBoardMount.png}
        \caption{Ball Valve Board Mount}
    \end{subfigure}

\end{figure}

\subsection{System Function}
\setlength{\parindent}{2em}
\setlength{\parskip}{1em}

The primary focus of the structures side of the fill station is three-fold. Firstly, the electronics in the fill station box must be securely mounted to the box to avoid damage. Secondly, the fill station box must have some measure in place to avoid overheating to prevent electronic failure. Finally, the fill station box must protect the electronics from dust while allowing for wires to pass through.

\noindent The board mounts are designed with heat set inserts embedded into the plastic to ensure that, once the boards are screwed into the mount, they remain secure. Each screw also has a plastic washer placed between the screw head and the electronic board to prevent damage from torquing of the screws. The mounts are secured to the board via VHB tape.

\noindent The dust covers are designed to be adhered to the box with red RTV adhesive to securely hold them in place as well as imrpove dust mitigation. Wires are able to pass through the mounts, but must be installed pre-RTV, to minimize areas that dust can get into the box. The mounts are tight enough to hold the wires in place without a large gap for open air, but also lose enough to allow for pulling of the wires in and out of the box for improved reach. 

\noindent The exterior of the box is also painted white to absorb less thermal radiation from the sun. This is by far the largest source of heat coming into the box, and the white paint mitigates this in a reliable and durable way. The box will also be set on a wooden stand at competition, so the bottom of it is not in contact with the hot sand. 

\subsection{Requirements}
\begin{table}[H]
\caption{\textbf{Structural Design Requirements}}
\label{tab:structural_requirements}
\centering
\renewcommand{\arraystretch}{2.5}

\begin{tabular}{|c|
>{\centering\arraybackslash}m{6cm}|
>{\centering\arraybackslash}m{3cm}|
>{\centering\arraybackslash}m{4cm}|}
\hline

\textbf{} &
\textbf{Requirement} &
\textbf{Reasoning} &
\textbf{Met} \\

\hline

1 &
Boards are easy to mount and remove &
Ease of Assembly &
Accomplished via heat-set inserts and screws \\

\hline

2 &
All PCB external ports should be accessible &
External Accessibility &
Dust covers provide wire-pass throughs\\

\hline

3 &
Boards must be secured &
Safety of Boards During Transport &
Accomplished via heat-set inserts and screws \\

\hline

4 &
Boarding housing dimensions must fit within the dimensions of the provided box &
System Integration &
System is designed to fit within designated box \\

\hline

5 &
All external electrical must allow minimal space for dust to enter &
Dust-Caused Short Circuits &
Red RTV holds covers in place and securely seals holes \\

\hline

6 &
Heat mitigation measures &
Electronic Overheating &
Box is painted white and will be on a stand \\

\hline

\end{tabular}

\end{table}

\subsection{Design}
The system has been designed to meet all of the aforementioned requirements. The board mounts have been designed to properly receive and securely hold heat set inserts, to ensure boards cannot go lose. Each screw also uses a plastic washer to prevent the screw from damaging the electrical boards. They have also been 3D printed with PETG due to its high glass transition temperature (roughly 170 Fahrenheit). The board mounts are secure to the box using VHB tape. Before the tape is applied, the area that will stick to the box is sanded down, to approve surface adhesion. The area the tape will sit is also sterilized with isopropyl alcohol to ensure that the board mount is properly attached to the box. 

\noindent The layout of the boards within the box was worked out with the electrical and software sub teams, to ensure logical and convenient placement of each board. The wire pass throughs were designed to minimize how much space there was in each wire pass through for dust to get in, and secured with red RTV to ensure the covers do not move easily. 

\noindent The exterior of the box has also been painted white, to minimize the solar radiation heating up the box. It will also be placed on a raised platform, so the box is not in direct contact with the hot sand to prevent conduction from being a major source of heat coming into the box. 

\subsection{System Analysis}
The only major analysis to be done on this system was a thermodynamic calculation, to verify that the current heat-mitigation measures should be enough to prevent overheating of the internal components in the box. 

\noindent The First Law of Thermodynamics yields the surface temperature of the box is equal to the following formula. This is assuming the only source of heat is the sun. The following assumptions can be made. Firstly, at the competition the box will not receive a significant amount of heat from convection because it is raised. Secondly, calculations were ran on heat produced from the electronics. Using Ohm's Law, it was found that at an amperage of 1.5 amps and voltage of 36 volts, both values much higher than the real electronics run on, the heat provided from these electronics assuming all of the energy was released as heat energy was one-tenth that of the heat from solar radiation.

\[
\alpha G A_{\text{sun}} - \varepsilon \sigma \left( T_s^4 - T_{\text{air}}^4 \right) - h A_{\text{box}} \left( T_s - T_{\text{air}} \right) = 0
\]

\[
\begin{array}{|c|l|}
\hline
\textbf{Variable} & \textbf{Meaning} \\
\hline
\alpha & \text{Solar absorptivity of the surface (dimensionless)} \\
G & \text{Solar irradiance (W/m}^2\text{)} \\
A_{\text{sun}} & \text{Projected area exposed to solar radiation (m}^2\text{)} \\
\varepsilon & \text{Emissivity of the surface (dimensionless)} \\
\sigma & \text{Stefan--Boltzmann constant } (5.67 \times 10^{-8}\ \text{W/m}^2\text{K}^4) \\
T_s & \text{Surface temperature (K)} \\
T_{\text{air}} & \text{Ambient air temperature (K)} \\
h & \text{Convective heat transfer coefficient (W/m}^2\text{K)} \\
A_{\text{box}} & \text{Convective surface area of the box (m}^2\text{)} \\
\hline
\end{array}
\]

\noindent Governed by this equation, the only design criteria at this point became emissivity and absorptivity of the box. It was found that for glossy white paint, the emissivity is roughly equal to 0.7 and the absorptivity was roughly 0.1. Using these values, combined with typical values for all other the other variables in Midland, Texas, it was found that the new maximum temperature of the box is roughly 118 degrees Fahrenheit. 

\[
\alpha \approx 0.1, \qquad
\varepsilon \approx 0.7, \qquad
T_{\max} = 118^\circ \mathrm{F} \approx 30.0^\circ \mathrm{C}
\]

\noindent This temperature is well below the previously found max temperature of 185 degrees Fahrenheit, and also below the maximum allowed temperature of the electronics of 140 degrees Fahrenheit. So, white glossy paint was used to paint the box, as it provided a heat-mitigation system that is reliable, durable, and easy to install.

\subsection{Testing}
\noindent The system was tested alongside the LV, and iterations were made through hot-fire and wet-dress tests based on feedback from the electrical and software sub teams. For example, when some mounts came loose during one test, the procedure around VHB tape was updated to include sanding and isopropyl alcohol disinfectant. This system was tested and validated in the field. This type of testing was the only option, as the facilities to test the thermal properties of the box are not available to our team. If there was some method available to mimic the radiation from the sun, it would be useful for testing the effects of sunlight on the internal temperature of the box. 

\subsection{Manufacturing}
\noindent The system was manufactured with input from the electrical and software sub teams on location of the board mounts. These teams were consulted pre-mount installation on where each mount should be mounted. The location of each mount was first sanded down with roughly 120-220 grit sandpaper and wiped down with an isopropyl alcohol wipe. This was done to improve surface adhesion with the VHB tape by increasing the surface area of the bond and cleaning the surface. The board mounts were then installed into the box using double-sided VHB tape. 

\noindent The fill station box already had pre-existing holes, so the dust covers and wire pass-throughs were designed to fit in these existing holes. For dust covers without a wire pass through, manufacturing consists of sliding the cover into the hole and using red RTV to secure it. For dust covers with wire pass-throughs, the wires must be slid through the hole then inserted into the designated notch in each cover. From there the dust cover can then be inserted into its hole and secured with red RTV. 

\noindent The board mounts and dust covers were 3D printed, and the board mounts had heat-set inserts melted into them. 

\noindent Painting the fill station box was done in a two-step process. First, two coats of primer were spray-painted onto the box. During this process, any holes in the box were covered with painters tape. After letting the primer sit for at least forty-eight hours, the paint could be applied. The paint was hand-painted on with a brush. Two coats of paint were used and painters tape was used to cover up any holes in the box.

\noindent The board mounts were installed first, the box was then painted, and finally the dust covers will be installed after final ground station electronics assembly at the competition. 

\subsection{Supply Chain}
The bill of materials for this project is included below. The fill station box was already in possession of the team and the dust covers and board mounts were 3D printed with pre-exisitng team resources. 

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.2}

\begin{tabular}{|l|l|l|l|c|}
\hline
\textbf{Name} & \textbf{Supplier} & \textbf{Quantity} & \textbf{Price} & \textbf{Received} \\ \hline

VHB Tape (1/2") & Amazon & 1 15 ft Roll & \$22.46 & Yes \\ \hline
White Paint (Behr Ultra-White) & Home Depot & 1 Gallon & \$50.94 & Yes \\ \hline
Heat-Set Inserts & McMaster & 2 packages & \$15.22 & Yes \\ \hline
Plastic Primer & McMaster & 2 cans & \$14.98 & Yes \\ \hline
Screws (2-56, 3/16") & McMaster & 1 package & \$4.19 & Yes \\ \hline
Paintbrush & McMaster & 1 piece & \$7.47 & Yes \\ \hline
Screws (2-56, 1/2") & McMaster & 1 package & \$3.50 & Yes \\ \hline
Nuts (2-56) & McMaster & 1 package & \$3.33 & Yes \\ \hline
Plastic Washers & McMaster & 1 package & \$12.12 & Yes \\ \hline

\end{tabular}

\caption{Bill of Materials and Procurement Status}
\label{tab:bom}
\end{table}

\noindent There were no sponsorships involved in this project and also no difficulties procuring any necessary items. 
