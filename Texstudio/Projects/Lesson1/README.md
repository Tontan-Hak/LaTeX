# Code 

``
\documentclass[12pt,a4paper]{book}
\usepackage[margin=1cm,includehead,includefoot]{geometry}
\usepackage[T1]{fontenc}
\usepackage[utf8]{inputenc}
\usepackage{xltxtra}
\defaultfontfeatures{Mapping=tex-text}
\XeTeXlinebreaklocale ”khm”
\XeTeXlinebreakskip = 0pt plus 1pt minus 1pt
%  ការប្រកាសកញ្ចប់កូដសំខាន់ៗមួួយចំនួន
\usepackage{sectsty}
\usepackage{amsmath}
\usepackage{amsfonts}
\usepackage{amssymb}
\usepackage{mathtools}
\usepackage{tikz}
\usepackage{tkz-tab}
\usepackage{varwidth}
\usepackage{enumerate}
\usepackage{enumitem}
\usepackage{multicol}
\usepackage{tasks}
\usepackage{framed}
\usepackage[framemethod=TikZ]{mdframed}
\usepackage[most]{tcolorbox}
\usepackage{tcolorbox}
\usepackage{xcolor}
\usepackage{graphicx}
\usepackage{rotating}
\usepackage{pgfornament}
\usetikzlibrary{patterns}
\usetikzlibrary{backgrounds}
\usepackage{eso-pic} 
\usepackage{float}
\usepackage{fontspec}
\usepackage{textcomp}
\usepackage{tkz-tab}
\tcbuselibrary{skins}
\usetikzlibrary{calc}
\usetikzlibrary{decorations.pathmorphing}
\usetikzlibrary{shadows.blur}
\usetikzlibrary{shapes.multipart}
 \usepgflibrary[shapes.misc] 
\usetikzlibrary{shapes.callouts}
\usepgflibrary{shapes.symbols} 
\usepackage{pgfornament}
\usepackage{pifont}
\usepackage{fontawesome5}
\usetikzlibrary{patterns}
\usepackage{pgfplots}
\pgfplotsset{compat=1.15}
\usepackage{mathrsfs}
\usetikzlibrary{arrows}
\usepackage{setspace}
\setstretch{1.2}
\everymath{\displaystyle}
\setmathrm{Times New Roman}
%  ការកំណត់ font គណិតវិទ្យាថ្មី
\usepackage[upint, smallerops]{newpxmath}
% ការកំណត់ font ខ្មែរសំខាន់ៗដែលត្រូវប្រើ
\setmainfont[Scale=0.875,AutoFakeBold=2,AutoFakeSlant=0.3]{Times New Roman}
\newcommand{\EN}{\fontspec{Times New Roman}\selectfont}
% ការកំណត់ពណ៌មួយចំនួនដែលត្រូវប្រើ
\definecolor{battleshipgrey}{rgb}{0.52, 0.52, 0.51}
\definecolor{azure(colorwheel)}{rgb}{0.0, 0.5, 1.0}
\definecolor{green-yellow}{rgb}{0.68, 1.0, 0.18}
\definecolor{bulgarianrose}{rgb}{0.28, 0.02, 0.03}
\definecolor{pinegreen}{rgb}{0.0, 0.47, 0.44}
\definecolor{vanilla}{rgb}{0.95, 0.9, 0.67}
\definecolor{coralred}{rgb}{1.0, 0.25, 0.25}
\definecolor{internationalkleinblue}{rgb}{0.0, 0.18, 0.65}
\definecolor{frenchrose}{rgb}{0.96, 0.29, 0.54}
\definecolor{cinnabar}{rgb}{0.89, 0.26, 0.2}
\definecolor{lavender(web)}{rgb}{0.9, 0.9, 0.98}
\definecolor{royalblue(traditional)}{rgb}{0.0, 0.14, 0.4}
\definecolor{lightgreen}{rgb}{0.56, 0.93, 0.56}
\definecolor{mikadoyellow}{rgb}{1.0, 0.77, 0.05}
\definecolor{seashell}{rgb}{1.0, 0.96, 0.93}
\definecolor{ceruleanblue}{rgb}{0.16, 0.32, 0.75}
\definecolor{frenchlilac}{rgb}{0.53, 0.38, 0.56}
\definecolor{pastelmagenta}{rgb}{0.96, 0.6, 0.76}
\definecolor{ruby}{rgb}{0.88, 0.07, 0.37}
\definecolor{oldmauve}{rgb}{0.4, 0.19, 0.28}
\definecolor{saffron}{rgb}{0.96, 0.77, 0.19}
\definecolor{teagreen}{rgb}{0.82, 0.94, 0.75}
\definecolor{darkbyzantium}{rgb}{0.36, 0.22, 0.33}
\definecolor{caribbeangreen}{rgb}{0.0, 0.8, 0.6}
\definecolor{crimson}{rgb}{0.86, 0.08, 0.24}
\definecolor{darkmidnightblue}{rgb}{0.0, 0.2, 0.4}
\definecolor{darkraspberry}{rgb}{0.53, 0.15, 0.34}
\definecolor{lavenderrose}{rgb}{0.98, 0.63, 0.89}
\definecolor{goldenyellow}{rgb}{1.0, 0.87, 0.0}
\definecolor{red(ncs)}{rgb}{0.77, 0.01, 0.2}
\definecolor{liver}{rgb}{0.33, 0.29, 0.31}
\definecolor{skobeloff}{rgb}{0.0, 0.48, 0.45}
\definecolor{tangelo}{rgb}{0.98, 0.3, 0.0}
\definecolor{internationalorange}{rgb}{1.0, 0.31, 0.0}
\definecolor{tealblue}{rgb}{0.21, 0.46, 0.53}
\definecolor{byzantium}{rgb}{0.44, 0.16, 0.39}
\definecolor{blue(pigment)}{rgb}{0.2, 0.2, 0.6}
\definecolor{tearose(rose)}{rgb}{0.96, 0.76, 0.76}
\definecolor{whitesmoke}{rgb}{0.96, 0.96, 0.96}
\definecolor{oxfordblue}{rgb}{0.0, 0.13, 0.28}
%  ការកំណត់ពណ៌ស្រមោល
\definecolor{shadecolor}{rgb}{0.95, 0.95, 0.96}
%  ការកំណត់លេខរៀងខ្មែរ និងអក្សរក្រមខ្មែរឲ្យរត់ស្វ័យប្រវត្តិ
\makeatletter 
\def\@khmernum#1{\expandafter\@@khmernum\number#1\@nil} 
\def\@@khmernum#1{%
\ifx#1\@nil 
\else 
\char\numexpr#1+"17E0\relax 
\expandafter\@@khmernum\fi 
} 
\def\knum#1{\expandafter\@khmernum\csname c@#1\endcsname}
\def\khmernumeral#1{\@@khmernum#1\@nil}
\AddEnumerateCounter{\knum}{\@knum}{}
\makeatother
\makeatletter
\newcommand*{\kalph}[1]{%
\expandafter\@kalph\csname c@#1\endcsname%
}
\newcommand*{\@kalph}[1]{%
\ifcase#1\or ក\or ខ\or គ\or ឃ\or ង\or ច\or ឆ\or ជ\or ឈ\or ញ\or  ដ\or ឋ\or ឌ\or ឍ\or ណ\or ត\or ថ\or ទ\or ធ\or ន\or ប\or ផ\or ព\or ភ\or ម\or យ\or រ\or ល\or វ\or ស\or ហ\or ឡ\or អ%
\else\@ctrerr\fi%
}
\AddEnumerateCounter{\kalph}{\@kalph}{}
\makeatother
% ការរចនាក្បាល និងជើងទំព័រនីមួយៗ
\usepackage{fancyhdr}
\pagestyle{fancy}
\fancyhf{}
\chead{
\tikz\draw[overlay,rounded corners=5pt,line width=1pt,black!75,fill=black!75](-0.49\textwidth,-0.41) rectangle (0.54\textwidth,1.14);
\tikz\draw[overlay,rounded corners=5pt,line width=1pt,darkmidnightblue,fill=seashell!50](-0.5\textwidth,-0.4) rectangle (0.53\textwidth,1.2);
\tikz\draw[overlay,rounded corners=5pt,line width=1pt,ruby,fill=lavenderrose!8](-0.2\textwidth,-0.1) rectangle (0.23\textwidth,0.9);
\tikz\node at (0,0.4)[overlay,black]{\large \textcolor{red(ncs)}{\EN Lesson}}; 
\tikz\node at (-0.50\textwidth,0.69)[overlay,black,anchor=west]{ \textcolor{oxfordblue}{\faBook \hspace{0.2cm}\EN Grade:}}; 
\tikz\node at (-0.506\textwidth,0)[overlay,black,anchor=west]{ \textcolor{oxfordblue}{\faGraduationCap \hspace{0.2cm} \EN Year:}}; 
\tikz\node at (0.39\textwidth,0.69)[overlay,byzantium]{\EN \textcolor{oxfordblue}{{\fontsize{14}{16.8}\ding{45}} Prepare by:}}; 
\tikz\node at (0.39\textwidth,0.05)[overlay,byzantium]{\large \textcolor{oxfordblue}{\EN name}}; 
}
\lfoot{\EN Facebook}
\cfoot{\begin{tikzpicture}[overlay,remember picture]
 \draw [fill=purple,magenta!8,thick,rounded corners=.3ex] (-1.5,-0.32) rectangle (.39,.32); 
 \node[white] at (-.5,0){{\color{black} \EN Page }\hspace*{.05cm}\color{black} \EN\thepage};
\end{tikzpicture}}
\rfoot{\EN Telegram}
\renewcommand{\headrulewidth}{0pt}
\renewcommand{\footrulewidth}{1.5pt}
\renewcommand{\headrule}{\hbox to\headwidth{%
\color{blue}\leaders\hrule height \headrulewidth\hfill}}
\renewcommand{\footrule}{\hbox to \headwidth{\color{blue}\leaders\hrule height \footrulewidth\hfill}}
%ការកំណត់កូដសម្រាប់ប្រើលេខឬអក្សរឲ្យរត់ស្វ័យប្រវត្តិ
\SetEnumitemKey{I}{%
    label={\protect\tikz[baseline=-0.9ex]\protect\node[draw=coralred,thick,circle,minimum height=.5cm,inner sep=1pt,text=oxfordblue,fill=seashell]{\Roman*};},font=\EN}
\SetEnumitemKey{1}{%
    label={\protect\tikz[baseline=-0.9ex]\protect\node[draw=magenta,thick,circle,minimum height=.5cm,inner sep=1pt,text=oxfordblue,fill=seashell]{\arabic*};},font=\EN}
\SetEnumitemKey{a}{%
    label={\protect\tikz[baseline=-0.9ex]\protect\node[draw=black,thick,circle,minimum height=.5cm,inner sep=1pt,text=oxfordblue,fill=seashell]{\alph*};},font=\EN}
% -------------------- ការកំណត់និយមន័យ --------------------
% ------------------------------------------------------------
% ------------------------------------------------------------
\newtcolorbox{definition}{
 enhanced,breakable,
 before skip=0.8cm,after skip=0.8cm,
 bottom=0.5cm,colframe=crimson,coltitle=white,
 colback=coralred!4,boxrule=0.2mm,arc=0mm,leftrule=2mm,
 attach boxed title to top left={xshift=0cm,yshift*=0mm-\tcboxedtitleheight},
 varwidth boxed title*=-3cm,
 boxed title style={frame code={
 \coordinate (A) at (frame.north east);
 \coordinate (B) at (frame.south east);
 \path[fill=coralred](frame.north east)--([xshift=-2mm]frame.north west)--([xshift=-2mm]frame.south west)--(frame.south east) --([xshift=3mm]$(A)!0.5!(B)$)--cycle;
 \draw[white,line width=2pt]([xshift=-2mm]frame.north east)--([xshift=1mm]$(A)!0.5!(B)$)--([xshift=-2mm]frame.south east);
 \path[fill=coralred!50]([xshift=-2mm]frame.south west)--+(2mm,-2mm)|-cycle;
 },interior engine=empty,
 },
 title={\bf\color{white} \large Definition}}
% -------------------- ការកំណត់ទ្រឹស្ដីបទ --------------------
% ------------------------------------------------------------
% ------------------------------------------------------------
\newtcolorbox{theorem}{breakable,enhanced,detach title,blanker,title={Theorem},coltitle=white,
 boxsep=3mm,top=2mm,left=2mm,right=2mm
 ,before skip=1cm,after skip=0.6cm,
 overlay={\scoped[on background layer]{
 \draw[fill=red!60!blue!3,draw=none](interior.north west)rectangle(interior.south east);
 \draw[red!60!blue](interior.north west)|-(interior.south east);},\node[anchor=west,font=\bfseries,
 scale=1.2,above right,fill=darkraspberry,xshift=-2mm,yshift=-2mm,drop shadow] (1) at (interior.north west){\tcbtitle};
 },overlay first={\scoped[on background layer]{
 \draw[fill=red!60!blue!3,draw=none](interior.north west)rectangle(interior.south east);
 \draw[red!60!blue](interior.north west)--(interior.south west);},\node[anchor=west,font=\large\bfseries,
 scale=1.2,above right,fill=red!60!blue,xshift=-2mm,yshift=-2mm,drop shadow] (1) at (interior.north west){\tcbtitle};
 },overlay middle={\draw[fill=red!60!blue!3,draw=none](interior.north west)rectangle(interior.south east);
 \draw[red!60!blue](interior.north west)--(interior.south west);},overlay last={\draw[fill=red!60!blue!3,draw=none](interior.north west)rectangle(interior.south east);
 \draw[red!60!blue](interior.north west)|-(interior.south east);}}
% -------------------- ការកំណត់ជាទូទៅ --------------------
% ------------------------------------------------------------
% ------------------------------------------------------------
\newtcolorbox{general}[1][]{
 enhanced,
 skin=enhancedlast jigsaw,
 attach boxed title to top left={xshift=-4mm,yshift=-0.5mm},
 fonttitle=\bfseries\sffamily,
 colbacktitle=blue,
 colframe=blue,
 interior style={
 top color=blue!5,
 bottom color=magenta!5
 },
 boxed title style={
 empty,
 arc=0pt,
 outer arc=0pt,
 boxrule=0pt
 },
 underlay boxed title={
 \fill[blue!65!white] 
 (title.north west) -- 
 (title.north east) -- 
 +(\tcboxedtitleheight-1mm,-\tcboxedtitleheight+1mm) -- 
 ([xshift=4mm,yshift=0.5mm]frame.north east) -- 
 +(0mm,-1mm) -- 
 (title.south west) -- cycle;
 \fill[blue!45!white!50!black] 
 ([yshift=-0.5mm]frame.north west) -- 
 +(-0.4,0) -- 
 +(0,-0.3) -- cycle;
 \fill[blue!45!white!50!black] 
 ([yshift=-0.5mm]frame.north east) -- 
 +(0,-0.3) -- 
 +(0.4,0) -- cycle; 
 },
 title={\large Generally},
 #1}
% -------------------- ការកំណត់លំហាត់គំរូ --------------------
% ------------------------------------------------------------
% ------------------------------------------------------------
\definecolor{bancolor}{RGB}{62,96,111}
\tcbset{myboxstyle/.style={enhanced,skin=enhanced jigsaw,
 attach boxed title to top left={xshift=-3mm,yshift=-\tcboxedtitleheight/2},
 coltitle=black,varwidth boxed title=0.7\linewidth,
 colbacktitle=#1!75, colback=caribbeangreen!5,sharp corners,
 top=2ex,
 boxed title style={sharp corners, boxrule=0pt},
 underlay boxed title={
 \fill[#1] (title.south west) -- (title.south-|frame.west)--++(0,-.2*\tcboxedtitleheight)--cycle;
 \fill[#1] (title.north east) --++(-.5*\tcboxedtitleheight,0)--++(0,.2*\tcboxedtitleheight)--cycle;}},
 myboxstyle/.default=teagreen}
\newtcolorbox[auto counter,number format=\arabic]{exercise}{myboxstyle,breakable,title={\faEdit Exercise \thetcbcounter},before skip=0.1cm,after skip=3mm, colframe=caribbeangreen}
% -------------------- ការកំណត់ដំណោះស្រាយ--------------------
% ------------------------------------------------------------
% ------------------------------------------------------------
\newtcolorbox{solution}[1][]{
 colframe=pastelmagenta,
 colback=pastelmagenta!12!white,
 boxed title style={colback=pastelmagenta},
 breakable,
 enhanced,
 sharp corners,
 boxsep=1pt,
 attach boxed title to top left={yshift=-\tcboxedtitleheight,  yshifttext=-1.05\baselineskip},
 boxed title style={boxsep=1pt,sharp corners},
 fonttitle=\bfseries\sffamily,
 no shadow,
 top=1ex,
 boxrule=0pt,
 leftrule=1.4pt,
 title={\color{darkbyzantium} Solution \fontsize{14}{16.8}\ding{45}},
 colframe=pastelmagenta,
 colback=pastelmagenta!12!white,
 boxed title style={colback=pastelmagenta},
 overlay unbroken and first={
 \node[below right,font=\small,color=magenta,text width=.8\linewidth]
 at (title.north east) {#1};
}}
% -------------------- ការកំណត់រំឮក---------------------
% ------------------------------------------------------------
% ------------------------------------------------------------
\newtcolorbox{review}{breakable,enhanced,colback=goldenyellow!5,colframe=goldenyellow,coltitle=black,title=\faLightbulb \hspace{0.2cm} Review,top=2mm,boxsep=3mm,
 attach boxed title to top left=
 {yshift=-\tcboxedtitleheight/2 ,xshift=0.3cm},
 boxed title style={size=small,colback=goldenyellow}}
% -------------------- ការកំណត់វិធាន  ---------------------
% ------------------------------------------------------------
% ------------------------------------------------------------
\newtcolorbox{way}{breakable,enhanced,colback=liver!5,colframe=liver,title=Way,top=2mm,boxsep=3mm,
 attach boxed title to top left=
 {yshift=-\tcboxedtitleheight/2 ,xshift=0.3cm},
 boxed title style={size=small,colback=liver}}
% -------------------- ការកំណត់លក្ខណៈ  ---------------------
% ------------------------------------------------------------
% ------------------------------------------------------------
\newtcolorbox{property}{breakable,enhanced,colback=skobeloff!5,colframe=skobeloff,title=Property,top=2mm,boxsep=3mm,
 attach boxed title to top left=
 {yshift=-\tcboxedtitleheight/2 ,xshift=0.3cm},
 boxed title style={size=small,colback=skobeloff}}
% -------------------- ការកំណត់សម្គាល់ ---------------------
% ------------------------------------------------------------
% ------------------------------------------------------------
\newtcolorbox{notation}{breakable,enhanced,colback=tangelo!5,colframe=tangelo,title=\faInfoCircle \hspace{0.1cm}Notation,top=2mm,boxsep=3mm,
 attach boxed title to top left=
 {yshift=-\tcboxedtitleheight/2 ,xshift=0.3cm},
 boxed title style={size=small,colback=tangelo}}
% -------------------- ការកំណត់ប្រតិបត្តិ ---------------------
% ------------------------------------------------------------
% ------------------------------------------------------------
\newtcolorbox[auto counter,number format=\arabic]{problem}{breakable,enhanced,title={Practice\thetcbcounter \hspace{0.1cm}\faSearch },
 colframe=tealblue,colback=blue!5,colbacktitle=tearose(rose)!25,
 fonttitle=\bfseries,coltitle=black,attach boxed title to top center=
 {yshift=-0.25mm-\tcboxedtitleheight/2,yshifttext=2mm-\tcboxedtitleheight/2},
 boxed title style={boxrule=0.5mm,
 frame code={ \path[tcb fill frame] ([xshift=-4mm]frame.west)
 -- (frame.north west) -- (frame.north east) -- ([xshift=4mm]frame.east)
 -- (frame.south east) -- (frame.south west) -- cycle; },
 interior code={ \path[tcb fill interior] ([xshift=-2mm]interior.west)
 -- (interior.north west) -- (interior.north east)
 -- ([xshift=2mm]interior.east) -- (interior.south east) -- (interior.south west)
 -- cycle;}}}
% -------------------- ការកំណត់សង្ខេប ---------------------
% ------------------------------------------------------------
% ------------------------------------------------------------
\newtcolorbox[auto counter]{summary}{breakable,top=1cm,title={Summary},enhanced,before skip=5mm,after skip=5mm,boxsep=3mm,colback=whitesmoke,coltitle=white,attach boxed title to top left={xshift=5mm,yshift=-\tcboxedtitleheight},boxrule=.5pt,boxed title style={interior empty,frame code={
\fill([xshift=1mm]frame.north east)arc(180:0:1mm)([xshift=-1mm]frame.north west)arc(0:180:1mm);
 \path[right color=cinnabar,left color=cinnabar,middle color=cinnabar!80] ([shift={(-.2,.1)}]frame.north west)--([shift={(.2,.1)}]frame.north east)[rounded corners=1mm]--([xshift=.1cm]frame.north east)--(frame.south east)--(frame.south west)--([xshift=-.1cm]frame.north west)[sharp corners]--cycle;}}}
% -------------------- ការកំណត់ប្រអប់ទំនើប ---------------------
% ------------------------------------------------------------
% ------------------------------------------------------------ 
\DeclareTColorBox{boxe}{ O{black} O{df}}{enhanced,breakable,
 before skip=2mm,after skip=0.3cm,
 bottom=0.5cm,colframe=#1,
 colback=#1!2,boxrule=0.2mm,arc=2mm,drop midday shadow=#1,
 attach boxed title to top left={xshift=0cm,yshift*=0mm-\tcboxedtitleheight},
 varwidth boxed title*=-3cm,
 boxed title style={frame code={
 \path[fill=#1]
 ([xshift=+0.5cm]frame.north east)[rounded corners=2mm]--(frame.north west)[sharp corners]--(frame.south west) --(frame.south east)to[out=0,in=180]cycle;
 \draw[#1]([yshift=-0.5mm]frame.south west)--([yshift=-0.5mm,xshift=+0.4mm]frame.south east)to[out=0,in=180]([yshift=0mm,xshift=+0.58cm]frame.north east);
 },interior engine=empty,
 },title={\large\bf #2},pad at break*=4mm}
% -------------------- ការកំណត់ប្រអប់សាមញ្ញ ---------------------
% ------------------------------------------------------------
% ------------------------------------------------------------ 
\newtcolorbox[auto counter,number within=section]{boxs}{
 enhanced,
 breakable,
 arc=0pt,
 outer arc=0pt,
 rightrule=2pt,
 toprule=0pt,
 bottomrule=0pt,
 leftrule=2pt,
 colframe=blue,
 colback=pink!20!,%drop lifted shadow,
 attach boxed title to top left,
 boxed title style={colback=blue,arc=0pt,outer arc=0pt,colupper=white}
}
% -------------------- ការកំណត់ប្រអប់ក្រដាស -------------------
% ------------------------------------------------------------
% ------------------------------------------------------------ 
\newtcolorbox{boxp}[1]{enhanced,
 interior code app={\fill[line width=1pt,draw=black,fill=gray!15 , blur shadow={shadow blur steps=1},shadow yshift=-0.2em,decoration={random steps,segment length=0.8cm,amplitude=.05cm},decorate]
 (frame.north west) -- (frame.north east) -- (frame.south east) -- (frame.south west) -- cycle;},frame hidden,
 fonttitle=\bfseries,top=0.4cm,
 attach boxed title to top left={yshift=-0.25mm-\tcboxedtitleheight/2,xshift=-0.7mm},
 boxed title style={enhanced,rotate=5,boxrule=.5mm,interior code app={\fill[line width=1pt,draw=black,fill=gray!15 , shadow yshift=-0.2em,decoration={random steps,segment length=0.8cm,amplitude=.05cm},decorate]
 (frame.north west) -- (frame.north east) -- (frame.south east) -- (frame.south west) -- cycle;}  },
 title={\large\color{red}#1}}
% -------------------- ការកំណត់ប្រអប់ឧទាន ---------------------
% ------------------------------------------------------------
% ------------------------------------------------------------ 
\newtcolorbox{remark}[1][]{enhanced,
 before skip=2mm,after skip=3mm,
 boxrule=0.4pt,left=5mm,right=2mm,top=1mm,bottom=1mm,
 colback=yellow!15,
 colframe=yellow!20!black,
 sharp corners,rounded corners=southeast,arc is angular,arc=3mm,
 underlay={%
 \path[fill=gray!80!black] ([yshift=3mm]interior.south east)--++(-0.4,-0.1)--++(0.1,-0.2);
 \path[draw,shorten <=-0.05mm,shorten >=-0.05mm] ([yshift=3mm]interior.south east)--++(-0.4,-0.1)--++(0.1,-0.2);
 \path[fill=yellow!50!black,draw=none] (interior.south west) rectangle node[white]{\large\bfseries !} ([xshift=4mm]interior.north west);
 },
 drop fuzzy shadow,#1}
% -------------------- ការកំណត់ប្រអប់លំហាត់ -------------------
% ------------------------------------------------------------
% ------------------------------------------------------------
\newtcolorbox[auto counter,number format=\knum]{exercise1}[1][]{%
 enhanced jigsaw,
 colback=seashell,%
 colframe=darkmidnightblue,
 size=small,
 boxrule=1.5pt,
 title=\KNR លំហាត់ទី\thetcbcounter,
 halign title=flush center,
 coltitle=ruby,
 breakable,
 drop shadow=black!50!white,
 attach boxed title to top left={xshift=1cm,yshift=-\tcboxedtitleheight/2,yshifttext=-\tcboxedtitleheight/2},
 minipage boxed title=3cm,
 boxed title style={%
 colback=pastelmagenta!25,
 size=fbox,
 boxrule=1.5pt,
 boxsep=2pt,
 underlay={%
 \coordinate (dotA) at ($(interior.west) + (-0.5pt,0)$);
 \coordinate (dotB) at ($(interior.east) + (0.5pt,0)$);
 \begin{scope}
 \clip (interior.north west) rectangle ([xshift=3ex]interior.east);
 \filldraw [pastelmagenta!25, blur shadow={shadow opacity=60, shadow yshift=-.75ex}, rounded corners=2pt] (interior.north west) rectangle (interior.south east);
 \end{scope}
 \begin{scope}[ruby]
 \fill (dotA) circle (2pt);
 \fill (dotB) circle (2pt);
 \end{scope}
 },
 },
 #1,
}

\parindent=0pt
\begin{document}
\begin{definition}
text text text text text text
\end{definition}
\begin{general}
text text text text text text
\end{general}
\begin{theorem}
text text text text text text
\end{theorem}
\begin{exercise}
text text text text text text
\end{exercise}
\begin{solution}
text text text text text text\\
text text text text text text
\end{solution}
\begin{review}
text text text text text text
\end{review}
\begin{way}
text text text text text text
\end{way}
\begin{property}
text text text text text text
\end{property}
\begin{notation}
text text text text text text
\end{notation}
\begin{problem}
text text text text text text
\end{problem}
\begin{summary}
text text text text text text
\end{summary}
\end{document}
```