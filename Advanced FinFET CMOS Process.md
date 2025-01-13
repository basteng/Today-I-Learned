
The previous section briefly explained how to build FinFET devices on a SOI wafer and on a bulk silicon wafer. It also described the gate-last HKMG process that replaces the polysilicon/SiON dummy gate with metal/high k. This section discusses in detail how to use advanced process technologies, such as SADP, ALD, etc., to form advanced HKMG FinFET CMOS devices on a bulk silicon substrate. 

The wafer is first cleaned, as shown in Fig. 3.9(a), and then a thin layer of pad oxide is thermally grown on the silicon surface, and a silicon nitride layer is deposited on the pad oxide. This SiN layer serves as a hard mask (HM) for the silicon etch that forms the fins of the FinFET; it also serves as a CMP stop layer during STI oxide polish. The fin pitch is too small to pattern an advanced-technology node (such as 22 nm or 14 nm) with one patterning of 193-nm immersion lithography, and thus SADP is needed. 

A dummy pattern layer of SADP is deposited on top of the nitride HM, and photoresist is coated on top of the entire stack [Fig. 3.9(b)]. The material of this layer needs to have high etch selectivity to the underlying silicon nitride and the spacer material that will be deposited on its sidewall to half the pitch and double the pattern density. One possible dummy/spacer-layer combination is a-Si/SiOx (amorphous silicon and silicon oxide). 

After PR patterning with a line-space fin dummy pattern mask, the dummy patterns, or mandrels, are etched with an endpoint at the SiN surface, as shown in Fig. 3.10(a). After PR strip and clean [Fig. 3.10(b)], a conformal dielectric layer is deposited [Fig. 3.10(c)], and then the dielectric layer is etched back in the vertical direction to form spacers on the sidewall of the mandrels, as shown in Fig. 3.10(d). After removal of the mandrels, the remaining spacer patterns form the line-space patterns that double the density of the original dummy pattern density [Fig. 3.10(e)]. If a-Si is used for the mandrels, potassium hydroxide (KOH) can be used to remove it with very little effect on the silicon oxide spacer and the underlying silicon nitride HM. The fin has the smallest pattern pitch of FinFET IC devices; advanced 14-nm IC chips have a fin pitch as small as 42 nm. 

After wafer clean, photoresist is coated on the wafer surface, and cut mask is applied to pattern the PR [Fig. 3.11(a)]. An anisotropic etch process is applied to remove the spacer pattern in the area where no fins are designed while keeping spacer patterns where the fins will be formed. This etch process needs high selectivity to the underlying nitride HM so that it etches away spacer patterns with minimal loss of the SiN HM. After PR strip and clean, the remaining spacer patterns can be used to etch SiN HM, as shown in Fig. 3.11(b). After etching away the pad oxide, the main etch process etches the silicon fin using SiN HM patterns [Fig. 3.11(c)]. 

![](/picture/Fig_3.9.png)

After wafer clean, an ILD layer is deposited [Fig. 3.12(a)], followed by ILD CMP with SiN as the endpoint [Fig. 3.12(b)]. After ILD recess, the SiN and pad oxide layer is stripped, as shown in Fig. 3.12(c). A sacrificial oxide layer is grown [Fig. 3.12(d)], a well-implantation mask is applied, ion implantation forms the isolation well between the channel and substrate, the sacrificial oxide is stripped, and wafer is cleaned, as shown in Fig. 3.12(e). This step finishes fin formation, which is somewhat similar to the STI formation of the planar CMOS process. As discussed earlier, it is critical to control the fin height because it directly affects the gate width of the FinFET devices.

![](/picture/Fig_3.10.png)

![](/picture/Fig_3.10_continue.png)

![](/picture/Fig_3.11.png)

![](/picture/Fig_3.12.png)

![](/picture/Fig_3.12_continue.png)

After fin formation, the wafer is cleaned, and a dummy gate oxide layer is deposited, followed by polysilicon deposition and CMP, as shown in Fig. 3.13(a). A HM layer is deposited, as shown in Fig. 3.13(b), and the gate mask is applied to form the line-space pattern on the photoresist. Depending on the technology node, if the gate pitch is larger than 80 nm, a single patterning with a 193-nm immersion lithography process can be used to form the line-space patterns. If the gate pitch is less than 80 nm, then pitchmultiplying techniques, such as SADP and SAQP, are needed. After HM etch and photoresist strip and clean, as shown in Fig. 3.13(c), a cut mask is applied, and an etch process cuts the HM line patterns. After that step, photoresist 
strip and clean occur, which form designed gate patterns on the HM layer [Fig. 3.13(d)]. This HM pattern is then used to etch polysilicon and form the dummy poly gate, as shown in Fig. 3.13(e).

![](/picture/Fig_3.13.png)

![](/picture/Fig_3.13_continue.png)

Now the fins and dummy polysilicon gate patterns are formed. The next processes are formation of S/D that involve spacer formation, ion implantation and selective epitaxial growth (SEG). 

After wafer clean, a thin dielectric liner is deposited, followed by a thicker dielectric layer [Fig. 3.14(a)]. A PMOS mask is applied so that the NMOS areas are covered by PR to allow S/D formation of the PMOS [Fig. 3.14(b)]. After PMOS spacer etch and fin-spacer removal, the photoresist is stripped and the wafer is cleaned [Fig. 3.14(c)]. Then silicon is recessed and heavily p-type doped SiGe is grown in a SEG process, as shown in Fig. 3.14(d). This finishes the PMOS formation.

![](/picture/Fig_3.14.png)

![](/picture/Fig_3.14_continue.png)

Next, NMOS S/D mask is applied, as shown in Fig. 3.15(a), NMOS spacer is etched and spacers on NMOS fins are removed [Fig. 3.15(b)]. N-type ion implantation is performed to heavily dope the NMOS S/D [Fig. 3.15(c)], and the photoresist is stripped and cleaned. Mini-second anneal (MSA) activated the dopant and finished the NMOS formation, as shown in Fig. 3.15(d). 

After the self-aligned silicide process forms silicide on the S/D, the wafer is ready for the replacement gate or gate-last HKMG process. First, the ILD1 is deposited, as shown in Fig. 3.16(a). Dielectric CMP removes part of the ILD1 to expose the dummy polysilicon gates [Fig. 3.16(b)]. After dummy-gate removal and oxide strip and clean, as shown in Fig. 3.16(c), hafnium-oxidebased high-k gate dielectric is deposited, followed by PMOS work-function 
metal TiN [Fig. 3.16(d)] and barrier metal TaN, all with ALD processes [Fig. 3.16(e)]. 

After wafer clean, photoresist is coated on the wafer, and a NMOS mask is applied to protect the PMOS and expose the NMOS, as shown in Fig. 3.17(a). An etch process removes the TaN barrier layer and TiN PMOS work-function metal, as shown in Fig. 3.17(b). After PR strip and clean, a NMOS work-function metal (such as TiAlN) is deposited [Fig. 3.17(c)]. A TiN adhesion layer is then deposited, followed by WCMP, which fills the gate trenches [Fig. 3.17(d)]. WCMP removes the bulk W. All other metal layers and the high-k dielectric layers are removed from the wafer surface in the over-polish step, as shown in Fig. 3.17(e).

This step finishes the FEoL of HKMG FinFET CMOS devices; the following steps are the middle-end-of-line (MEoL) processes. The processes of a 14-nm HKMG FinFET SRAM could have two layers with a total of four masks. One layer is the S/D contact (SDC) with two masks, and another layer is the gate contact (GC) with two masks. After two cycles of ILD/HM deposition, contact double patterning, contact etch, TiN and W deposition, and WCMP, the MEoL processes are finished; the contact plugs and local interconnection are formed, and the back-end-of-line (BEoL) processes could be started. Figure 3.18(a) is a transmission electron microscope (TEM) image of the cross-section of a 22-nm FinFET CMOS device with S/D contact and gate contact. Figure 3.18(b) is Fig. 3.17(e) with dashed lines to indicate the direction of the cross-section. The SDC contacts are not round holes but rather elongated trenches. The next section describes the processes of the contact module. 

![](/picture/Fig_3.15.png)

![](/picture/Fig_3.15_continue.png)

The BEoL processes start with wafer clean and etch-stop layer (ESL) deposition. They are followed by depositions of ultra-low-k dielectric, a cap oxide layer, TiN metal HM layer, dielectric HM layer, and the dummy layer. After inspection, review, and clean, PR is coated on the wafer, the first metal mask is applied, and mandrels are etched from the dummy layer. A conformal dielectric layer is deposited, and an etch-back process forms spacers on the sidewalls of the mandrels. After mandrel removal, the pitch of the line space is halved. The cross-section along the spacer is shown in Fig. 3.19(a). The process steps are very similar to that illustrated in Fig. 3.10. A cut mask is applied, and the looped lines formed by the spacer are cut into the designed pattern, as shown in Fig. 3.19(b). A dielectric layer is deposited to fully cover the patterns, illustrated in Fig. 3.19(c). A CMP process planarizes the dielectric and exposes the patterns that are embedded in the dielectric film [see Fig. 3.19(d)]. A highly selective etch process removes the embedded patterns to form the dielectric HM etch, which can be used to etch the TiN hard mask, as shown in Fig. 3.19(e). 3D illustrations of this pattern reversal process are shown in Fig. 3.18(f). After dielectric HM strip and clean, the M1 trench patterns are transferred to TiN hard mask. Next, the V1 mask is applied, and the V1 is etched when it is aligned with M1, as shown in Fig. 3.19(i). After the via hole reaches the ESL, etch is stopped and PR is stripped. Trenches are etched using a TiN HM, and the ESL is broken through at the bottom of via holes [Fig. 3.19(j)]. After barrier TaN and seed Cu deposition, bulk Cu is plated, shown in Fig. 3.19(k). The wafer is then cleaned and annealed. Metal CMP removes the Cu, TaN, and TiN metal HM from the wafer surface, and self-aligned cobalt tungsten phosphide (CoWP) is deposited on the metal surface with an electrode-less plating process, as shown in Fig. 3.19(l). This step finishes the dual-damascene M1 process module.

![](/picture/Fig_3.16.png)

![](/picture/Fig_3.16_continue.png)

![](/picture/Fig_3.17.png)

![](/picture/Fig_3.17_continue.png)

If V1 is not well aligned with M1, then the TiN hard mask could block the V1 etch, creating a small via hole and void in the via plug after metal deposition, as in Fig. 3.20. The small via could also be caused by the pull-back of the trench pattern. Sometimes a small via cannot be etched all the way to the previous metal layer, which causes an open circuit of the interconnect. 

The M2, M3, and Mx layers essentially repeat the M1 process steps (x is the number of total metal layers). There are 13 metal layers for a 14-nm FinFET CMOS chip—the most-advanced IC technology node in highvolume manufacturing at the time of publication. The main variations are the upper metal layers, which have a larger feature size and thus do not require double patterning. The feature sizes of the last few metal layers become so large that they do not require 193-nm immersion lithography; 248-nm (KrF excimer laser) or even 365-nm (i-line of a mercury lamp) lithography could be used. Figure 3.21 shows a cross-section of a 13-metallayer HKMG FinFET chip.17

![](/picture/Fig_3.18.png)







