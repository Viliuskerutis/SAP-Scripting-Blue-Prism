# SAP-Scripting-Blue-Prism

## Teikiamos funkcijos
	Sukurtas komponentas leidžia palengvinti SAP (angl. Systems Applications and Products in Data Processing) sistemos automatizavimą. Komponentas įtraukia dažniausiai SAP sistemoje naudojamus veiksmus tokius kaip: mygtuko paspaudimas, lentelės nuskaitymas, reikšmių įvedimas, žymėjimas ir daugybė kitų. Naudojant Blue Prism programinę įrangą tereikia iš SAP sistemos gauti norimo automatizuoti elemento unikalų kodą ir įrašyti jį į atitinkamo veiksmo laukelį.
## Paskirtis
	Sukurtas komponentas įtrauktas į RPA (angl. Robotic Process Automation) projektą padeda lengvai, greitai ir stabiliai automatizuoti SAP programą.
## Sprendžiamos problemos
	Programos, sukurtos naudojant siūlomą komponentą, automatizuos fizinių asmenų atliekamą darbą su SAP programa. Taigi, žmonėms nebereikės atlikti užduočių patiems, bus sutaupomas laikas ir, žinoma, resursai – tiek žmogiškieji, tiek finansiniai.
	Iš automatizavimo pusės sprendžiama patogumo, greičio ir stabilumo stokos problema. Seniau SAP buvo automatizuojamas kitais, universaliais metodais, su kuriais galima automatizuoti ir SAP, ir naršykles, ir darbalaukio programas. Tai patogu, nes vienas metodas yra tinkamas daugeliui atvejų, tačiau tai nėra itin patogu bei stabilu, kai norima automatizuoti išskirtinai SPA programą. Automatizuotos programos dirbdavo beveik tiek pat laiko, kiek ir fiziniai asmenys, dažnai užstrigdavo ir nebuvo itin stabilios. Šis komponentas išsprendžia šią bėdą, nes yra sukurtas išskirtinai SAP automatizavimui, yra patogus naudojimui, automatizuotos programos veikia itin greitai ir stabiliai.
## Naudojimosi tikslai
	Automatizuojant programas nėra vieno teisingo būdo kaip tai galima padaryti. Vieni variantai saugesni, tačiau lėti, kiti greiti, tačiau nestabilūs. Šis komponento tikslas yra automatizuoti SAP platformą greitai ir saugiai, išvengiant bereikalingų laukimo funkcijų. Visi veiksmai yra vykdomi iškart, kai tik prieš tai buvęs veiksmas yra atliekamas. Tai vyksta savaime ir komponento naudotojas neturi tuo rūpintis. Komponento darbo su SAP sistema greitaveika yra bent dešimt kartų greitesnė lyginant su fizinio asmens darbo greičiu su ta pačia sistema. Taigi, greitis ir naudojimosi paprastumas yra pagrindiniai šio komponento naudojimo tikslai.
## Apribojimai komponento naudojimui
	Šis komponentas automatizuoja SAP sistemos elementus, tačiau verta atkreipti dėmesį, kad kartais SAP viduje yra įdiegtų įskiepių, kurie tarsi yra SAP programos dalis, tačiau iš tikrųjų nėra realūs SAP elementai. Tai tarsi programos programoje. Tokių elementų šis komponentas automatizuoti negali, nes jie neturi SAP elemento unikalaus kodo, ir jų automatizavimui turėtų būti pasirinkti kiti sprendimai.
##	Kita svarbi informacija komponento vartotojui
	Nors komponente yra įtraukti visi dažniausiai naudojami elementai ir jų funkcijos, tačiau galima suprasti, kad SAP sistema yra itin didelė ir joje egzistuoja rečiau naudojamos funkcijos, kurios gali būti neįtrauktos į šį komponentą.
	SAP sistema turi daugybę posistemių ir komponentas visuose veikia.

## Detalūs funkcijų aprašai
	Žemiau pateiktoje lentelėje yra matomi visų funkcijų (veiksmų, klasių) aprašai. Nurodoma, ką kiekviena funkcija atlieka, jos rezultatas bei įvesties parametrų reikšmės.

#	Funkcija	Įvestis	Aprašas	Išvestis
1	press	•	Reference – unikalus elemento kodas gaunamas iš SAP sistemos.	Paspaudžia elementą. Dažniausiai naudojama mygtukų paspaudimams.	Elementas yra paspaudžiamas. Ekvivalentas pelės kairiojo klavišo paspaudimui.
2	pressButtonCurrentCell	•	Reference – unikalus elemento kodas gaunamas iš SAP sistemos.	Paspaudžia tuo metu aktyvų lentelės langelį. Dažniausiai naudojamas elementų lentelėse paspaudimams.	Aktyvus lentelės langelis yra paspaudžiamas. Ekvivalentas pelės kairiojo klavišo paspaudimui.
3	doubleClickCurrentCell	•	Reference – unikalus elemento kodas gaunamas iš SAP sistemos.	Du kartus paspaudžia tuo metu aktyvų lentelės langelį. Dažniausiai naudojamas elementų lentelėse paspaudimams.	Aktyvus lentelės langelis yra paspaudžiamas du kartus. Ekvivalentas pelės kairiojo klavišo paspaudimui.
4	pressToolbarButton	•	Reference – unikalus elemento kodas gaunamas iš SAP sistemos.
•	ButtonName – įrankių juostos mygtuko kodas.	Paspaudžia įrankių juostos mygtuką.	Įrankių juostos punktas yra pasirinktas. Ekvivalentas pelės kairiojo klavišo paspaudimui.
5	doubleClickItem	•	Reference – unikalus elemento kodas gaunamas iš SAP sistemos.
•	Row – eilutės numeris.
•	Column – stulpelio numeris.	Paspaudžia specifinį lentelės elementą du kartus. Dažniausiai naudojamas elementų lentelėse paspaudimams.	Specifinis lentelės elementas yra paspaudžiamas du kartus. Ekvivalentas pelės kairiojo klavišo paspaudimui.
6	pressContextButton	•	Reference – unikalus elemento kodas gaunamas iš SAP sistemos.
•	ButtonName – mygtuko pavadinimas.
•	MenuItem - meniu punkto mygtuko kodas.	Paspaudžia meniu mygtuką.	Meniu punktas yra pasirinktas. Ekvivalentas pelės kairiojo klavišo paspaudimui.
7	pressButton	•	Reference – unikalus elemento kodas gaunamas iš SAP sistemos.
•	ButtonName – mygtuko pavadinimas.	Paspaudžiamas specifinis mygtukas, turintis unikalų vardą.	Specifinis mygtukas yra paspaudžiamas. Ekvivalentas pelės kairiojo klavišo paspaudimui.
8	pressToolbarContextButton	•	Reference – unikalus elemento kodas gaunamas iš SAP sistemos.
•	ButtonName – mygtuko pavadinimas.	Paspaudžiamas meniu juostos mygtukas iš išskleidžiamo sąrašo. Dažniausiai naudojamas išskleidžiamų meniu elementų paspaudimams.  	Meniu juostos mygtukas iš išskleidžiamo sąrašo yra paspaudžiamas. Ekvivalentas pelės kairiojo klavišo paspaudimui.
9	selectedRows	•	Reference – unikalus elemento kodas gaunamas iš SAP sistemos.
•	Row_id – eilutės numeris.	Pažymima specifinė eilutė. Naudojamas išskirtinai lentelėse.	Specifinė eilutė yra pažymima.
10	selectColumn	•	Reference – unikalus elemento kodas gaunamas iš SAP sistemos.
•	ColumnName – stulpelio pavadinimas.	Pažymimas specifinis stulpelis. Naudojamas išskirtinai lentelėse.	Specifinis stulpelis yra pažymimas.
11	selected	•	Reference – unikalus elemento kodas gaunamas iš SAP sistemos.
•	Select – tiesa arba melas (angl. true or false) reikšmė.	Pažymimas arba atžymimas pasirinkimo langelis (angl. checkbox). Naudojamas išskirtinai tik su pasirinkimo langeliais.	Pasirinkimo langelis yra pažymimas arba atžymimas priklausomai nuo įvesties parametrų reikšmės.
12	getAbsoluteRow-selected	•	Reference – unikalus elemento kodas gaunamas iš SAP sistemos.
•	Row_id – eilutės numeris.	Grąžinama, ar specifinė eilutę pažymėta, ar ne. Naudojamas išskirtinai lentelėse.	•	Selected – tiesa arba melas (angl. true or false) reikšmė.
13	selectItem	•	Reference – unikalus elemento kodas gaunamas iš SAP sistemos.
•	Row – eilutės numeris.
•	Column – stulpelio unikalus kodas.	Pažymimas specifinis lentelės elementas. Naudojamas išskirtinai lentelėse.	Specifinis lentelės elementas yra pažymimas.
14	select	•	Reference – unikalus elemento kodas gaunamas iš SAP sistemos.	Pažymimas elementas. Naudojamas visiems kitiems elementams, kurie nėra lentelė, pasirinkimo langelis ar meniu punktas.	Elementas yra pažymimas.
15	selectContextMenuItem	•	Reference – unikalus elemento kodas gaunamas iš SAP sistemos.
•	MenuItem – meniu elemento unikalus kodas.	Pažymimas meniu punktas.	Meniu punktas yra pažymimas.
16	caretPosition	•	Reference – unikalus elemento kodas gaunamas iš SAP sistemos.	Grąžina elemento poziciją lange. Dažniausiai naudojamas lentelėse.	•	Pasition – elemento pozicija.
17	verticalScrollbar-position	•	Reference – unikalus elemento kodas gaunamas iš SAP sistemos.
•	Pasition – vertikaliosios slinkties juostos pozicijas.	Pakeičia vertikaliosios slinkties poziciją, t.y. paslenka ekrano vaizdą aukštyn arba žemyn.	Vertikaliosios slinkties pozicija yra pakeičiama. Ekrano vaizdas pasikeičia. Ekvivalentas pelės slinkties elemento naudojimui.
18	firstVisibleRow	•	Reference – unikalus elemento kodas gaunamas iš SAP sistemos.	Grąžina pirmos matomos eilutės poziciją. Naudojamas išskirtinai lentelėse.	•	Pasition – pirmos matomos eilutės pozicija.
19	horizontalScrollbar-position	•	Reference – unikalus elemento kodas gaunamas iš SAP sistemos.
•	Pasition – horizontaliosios slinkties juostos pozicijas.	Pakeičia horizontaliosios slinkties poziciją, t.y. paslenka ekrano vaizdą kairėn arba dešinėn.	Horizontaliosios slinkties pozicija yra pakeičiama. Ekrano vaizdas pasikeičia.
20	openSession	Papildomos įvesties šiai funkcijai nėra.	Atidaro naują sesijos langą.	•	ConnectionID – prisijungimo unikalus numeris.
•	SessionID – sesijos unikalus numeris.
21	currentCellColumn	•	Reference – unikalus elemento kodas gaunamas iš SAP sistemos.	Grąžina lentelės aktyvaus stulpelio pavadinimą.	•	ColumnName – stulpelio pavadinimas.
22	sendVKey	•	Window_id – aktyvaus lango unikalus numeris.
•	Value – sparčiojo klavišo ar jų kombinacijos skaitinis atitikmuo*.	Atlieka sparčiojo klavišo ar jų kombinacijos veiksmą, pavyzdžiui, Shift+F4.	Sparčiojo klavišo ar jų kombinacijos veiksmas yra atliekamas. 
23	text	•	Reference – unikalus elemento kodas gaunamas iš SAP sistemos.
•	Value – simbolių įvestis įrašymui.	Įrašo nurodytą tekstą (simbolių įvestį) į elementą. Naudojamas tik redaguojamiems (angl. editable, read-write) elementams.	Nurodytas tekstas įrašomas elemente.
24	readText	•	Reference – unikalus elemento kodas gaunamas iš SAP sistemos.	Nuskaito elemento tekstą. Naudojamas bet kokiems elementams, kurie savyje talpina informaciją.	•	Value – simbolių išvestis skaitymui.
25	setCurrentCell	•	Reference – unikalus elemento kodas gaunamas iš SAP sistemos.
•	Cell_Name
•	Cell_ID	Pasirenka specifinį lentelės elementą. Naudojamas išskirtinai lentelėse.	Specifinis lentelės elementas yra pasirenkamas.
26	currentCellRow	•	Reference – unikalus elemento kodas gaunamas iš SAP sistemos.	Grąžina lentelės aktyvios eilutės unikalų numerį.	•	Cell_ID – eilutės unikalus numeris.
27	key	•	Reference – unikalus elemento kodas gaunamas iš SAP sistemos.	Grąžina elemento unikalų raktą. Naudojamas tik su itin specifiniais elementais.	•	Key – elemento unikalus raktas.
28	getTable	•	Reference – unikalus elemento kodas gaunamas iš SAP sistemos.	Nuskaito norimos lentelės visus duomenis ir įrašo į kolekciją.	•	Output_Collection – nuskaitytos lentelės duomenys.
29	maximize	•	Window_id – aktyvaus lango unikalus numeris.	Išdidina norimo sistemos lango vaizdą.	Sistemos lango vaizdas yra išdidinamas.
30	setFocus	•	Reference – unikalus elemento kodas gaunamas iš SAP sistemos.	Sufokusuoja vaizdą ties norimu elementu.	Vaizdas ties norimu elementu yra sufokusuojamas.
*Sparčiųjų klavišų ar jų kombinacijų skaitinį atitikmenį galime matyti žemiau esančioje lentelėje.

VKey	Klaviatūros kombinacija	VKey	Klaviatūros kombinacija	VKey	Klaviatūros kombinacija
00	Enter	22	Shift+Ctrl+0	45	Ctrl+Shift+F9
01	F1	23	Shift+F11	46	Ctrl+Shift+F10
02	F2	24	Shift+F12	47	Ctrl+Shift+F11
03	F3	25	Ctrl+F1	48	Ctrl+Shift+F12
04	F4	26	Ctrl+F2	70	Ctrl+E
05	F5	27	Ctrl+F3	71	Ctrl+F
06	F6	28	Ctrl+F4	72	Ctrl+/
07	F7	30	Ctrl+F6	73	Ctrl+\
08	F8	31	Ctrl+F7	74	Ctrl+N
09	F9	32	Ctrl+F8	75	Ctrl+O
10	F10	33	Ctrl+F9	76	Ctrl+X
11	Ctrl+S	34	Ctrl+F10	77	Ctrl+C
12	F12	35	Ctrl+F11	78	Ctrl+V
13	Shift+F1	36	Ctrl+F12	79	Ctrl+Z
14	Shift+F2	37	Ctrl+Shift+F1	80	Ctrl+PageUp
15	Shift+F3	38	Ctrl+Shift+F2	81	PageUp
16	Shift+F4	39	Ctrl+Shift+F3	82	PageDown
17	Shift+F5	40	Ctrl+Shift+F4	83	Ctrl+PageDown
18	Shift+F6	41	Ctrl+Shift+F5	84	Ctrl+G
19	Shift+F7	42	Ctrl+Shift+F6	85	Ctrl+R
20	Shift+F8	43	Ctrl+Shift+F7	86	Ctrl+P
21	Shift+F9	44	Ctrl+Shift+F8		

