# The Imperative of Open Sourcing Chip Manufacturing Processes

The India Semiconductor Mission's (ISM) ambitious goal to establish a robust domestic chip design and manufacturing ecosystem is gradually achieving fruition. The Union government recently approved three semiconductor units, including India's first fabrication plant by Tata Electronics Private Limited, in partnership with Taiwan's Powerchip Semiconductor Manufacturing Corporation in Dholera, Gujarat.

 ![](https://substackcdn.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2F59219984-efcd-495a-8b05-17aedefe1cb3_641x423.png " =721x475")

**Foundation stone laying ceremony of the TATA-PSMC fab project (**Source**: [The Indian Express](https://indianexpress.com/article/business/tata-fab-to-roll-out-first-chip-by-2026-end-pm-calls-it-historic-9212483/))**

India's presence in the chip design stage of the global value chain (GVC) is sizeable and well-established, playing host to global semiconductor design houses such as AMD and Qualcomm. There's a slight glitch in the matrix, though: despite a large pool of skilled design engineers and a growing domestic market, India has struggled to establish a robust homegrown chip design and product ecosystem.

New Delhi has launched initiatives like the semiconductor Design-Linked Incentive (DLI) and Chips 2 Startup (C2S) schemes, which aim to provide select startups and universities with affordable access to Electronic Design Automation (EDA) software tools essential for designing all modern chips. (We have previously written about the issues surrounding the extant version of the DLI scheme [here](https://www.thehindu.com/opinion/op-ed/the-need-to-overhaul-a-semiconductor-scheme/article67768726.ece).)

However, a key hurdle for startups and academia is the lack of standardised and affordable access to collaborative research facilities and critical chip design toolkits inextricably linked to the fabrication stage of the supply chain that India is focused on: Process Development Toolkits (PDKs).

 ![](https://substackcdn.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2F37a40e08-daea-4722-b83c-a0c4fdd15ca6_1583x705.png " =1456x648")

**Figure 1**: Different elements of a PDK (Source: [Cadence](https://community.cadence.com/cadence_blogs_8/b/breakfast-bytes/posts/all-the-ps-the-photonics-pdk-panel))

A PDK is essentially a suite of files, libraries, and documentation provided by a semiconductor fabrication facility that contains detailed information about the manufacturing process, rules for design, models, and other technical specifications required to reliably design millions of chips.

Consider these as standardised building blocks adhering to the manufacturing constraints and capabilities of a foundry's specific process node (130nm, 65nm, etc.), which designers use to construct more complex chip layouts. Adhering to these rules is critical for fabless firms to achieve high yields and reliability in the final manufactured chips.

Foundries worldwide invest significant resources in developing and optimising their manufacturing processes. Their PDKs contain sensitive and proprietary information, so they are closely guarded and provided only to design firms under strict non-disclosure requirements and hefty licensing fees.

The proprietary nature of PDKs has some obvious drawbacks for a nascent industry and for academia's efforts to cultivate homegrown talent. It adds to the high costs of chip design and can create entry barriers for smaller design firms and startups who may not have the resources or relationships to access PDKs from commercial fabs.

Just designing a chip from scratch for a mature 65nm node alone costs almost [$25 to 30 million](https://semiengineering.com/what-will-that-chip-cost/). This can also limit collaboration and innovation in the design ecosystem, as designers are restricted in their ability to iterate and build upon each other's work if the prior work relied upon a specific fab's PDK. In academic institutions, students may study the theoretical foundations of advanced chip design but not gain practical expertise in[ manufacturable process flows](https://www.skywatertechnology.com/sky130-open-source-pdk/) that would make them valuable talent for design and fabrication facilities worldwide.

Proprietary/closed-source PDKs are a stumbling block for the proliferation of open-source hardware, as well as for the open-source community and researchers that develop accompanying EDA tools for such silicon. They pose a security question because countries want to ensure that chips for strategic and military purposes are sourced from trusted foundries; not being able to audit the code determining the layout of those chips is a potential vulnerability, as it could be an avenue for[ inserting](https://takshashila.org.in/research/a-survey-of-chip-based-hardware-backdoors) hardware backdoors.

Industry and academia worldwide have recognised these drawbacks, and some recent efforts to develop open-source PDKs are underway. SkyWater Open Source PDK, for example, was [released](https://www.skywatertechnology.com/sky130-open-source-pdk/) in 2020 as a collaboration between Google and SkyWater Technology Foundry. It aims to provide anyone with free access to a manufacturable PDK for SkyWater's 130nm process. Open source initiatives like this and Germany's IHP Open PDK have begun widening access to chip design by providing low-cost entry points to students, researchers, and small startups.

India's existing semiconductor research facilities in academic institutions like the Indian Institute of Science's (IISc) National Nanofabrication Centre, the Indian Institute of Technology, Bombay's (IIT-B) Nanofabrication facility, and the state-owned Semiconductor Research Laboratory (SCL) could provide startups and researchers everywhere with open access to their PDKs. Inexplicably, this has not happened. 

A potential open and collaborative model is [Australia's National Fabrication Facility ](https://anff.org.au/)and the [Canadian CMC Microsystems](https://www.cmc.ca/).

 ![](https://substackcdn.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2F3407028b-9d5b-4ae4-aa99-d1eae9810604_1068x940.png " =1068x940")

**Figure 2**: [ANFF has 8 Nodes spread across 21 institutions](https://anff-act.anu.edu.au/).

Like IISc and IIT-B, Australia's National Fabrication Facility (ANFF) also has state-of-the-art tooling and characterisation facilities. While it does not open-source its PDKs, it provides open access to its specialised fabrication and research facilities for prototyping, skill development, and training to all Australian researchers and industry clients for a fee. Similarly, Canada's CMC Microsystems is a non-profit that provides shared access to state-of-the-art design tools, prototype fabrication, testing capabilities, and expertise to researchers and industry worldwide via its National Design Network.

 ![](https://substackcdn.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2F2a07c4a8-20be-48b8-95a2-e2ad236fea28_787x509.png " =787x509")

**Figure 3**: Source - [CMC's Annual Report (2022-23)](https://www.cmc.ca/wp-content/uploads/2024/04/AnnualReport_2022-2023-EN.pdf)

CMC provides EDA tools and open-source PDKs to Canadian clients but also couples those with subsidised access to fabrication services through eight different partner foundries worldwide.

An equivalent model in India could function as a hub-and-spoke network with institutions like IISc and IIT-B functioning similarly to ANFF's nodes, offering open access to research facilities and R&D fabs (with open-source PDKs) to Indian researchers and industry. A consortium of such institutions could aggregate client designs and manage the fabrication process with SCL functioning as the foundry hub of the model. The union government's [recently unveiled](https://indiaeconomicclub.org/business-news-%26-insights/f/scl-resurrects-with-rs-10000-crore-modernization-plan?blogcategory=Semi+Conductors) INR 10,000cr plan to invest in SCL to transform it into an R&D centre could make this model a reality. Taking a page out of CMC's book, this model could look towards onboarding more trusted foundries from friendly countries like Singapore.

This effort can be subsidised under an existing or new ISM initiative or the recently announced [Indian Semiconductor Research Centre](https://economictimes.indiatimes.com/tech/technology/centre-eyes-dedicated-rd-wing-under-semicon-research-centre/articleshow/109958069.cms?from=mdr).

Such a model would accelerate semiconductor product development in India. It would enable researchers to verify novel concepts, startups to reduce time to market, and students to gain hands-on experience in manufacturable chip design—all while fostering a sorely needed culture of collaboration and innovation.

***\*\*Satya and Pranay are researchers with the High-Tech Geopolitics programme at the Takshashila Institution, Bangalore. For the latest research updates from Takshashila Institution, visit <https://takshashila.org.in/>\*\****

\n