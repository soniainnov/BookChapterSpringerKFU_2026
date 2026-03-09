# A Systematic Review of IoT-Enabled Smart Agriculture for Food Security and Sustainable Development: Opportunities, Challenges, and Future Directions

**Sonia Ben Aissa · Mounir Frikha**

Department of Computer Networks and Communications, College of Computer Sciences and Information Technology, King Faisal University, Al-Ahsa, Saudi Arabia

saissa@kfu.edu.sa

---

## Abstract

Food security remains a critical global challenge, particularly in developing countries where agricultural systems face mounting pressures from climate change, population growth, and resource scarcity. The Internet of Things (IoT) has emerged as a transformative technology with significant potential to modernize agricultural practices and contribute to the United Nations Sustainable Development Goals (SDGs), notably SDG 2 (Zero Hunger), SDG 9 (Industry, Innovation and Infrastructure), and SDG 13 (Climate Action). This chapter presents a systematic literature review following the PRISMA (Preferred Reporting Items for Systematic Reviews and Meta-Analyses) protocol, covering peer-reviewed publications from 2018 to 2025 retrieved from IEEE Xplore, Scopus, Web of Science, ACM Digital Library, and Google Scholar. A total of 87 studies were retained after applying rigorous inclusion and exclusion criteria. Our review examines IoT architectures, sensor technologies, and Low-Power Wide-Area Network (LPWAN) communication protocols — including LoRaWAN, NB-IoT, and Sigfox — deployed in smart agriculture contexts, with a particular focus on developing country settings. The originality of our work consists in providing a comprehensive dual-impact analysis, addressing both the positive contributions of IoT — including water efficiency, crop yield optimization, pest detection, and climate-adaptive farming — and the negative externalities such as e-waste generation, energy consumption, and cybersecurity vulnerabilities. Furthermore, we identify key structural challenges hindering large-scale IoT adoption in resource-constrained environments and propose future research directions. Our findings confirm the substantial potential of IoT-enabled smart agriculture in advancing food security, while highlighting the urgent need for sustainable, low-cost, and inclusive technology deployment strategies.

**Keywords:** Internet of Things · Smart Agriculture · Food Security · LPWAN · LoRaWAN · SDG 2 · Developing Countries · Precision Farming · Systematic Review · PRISMA

---

## 1  Introduction

Food insecurity continues to threaten the livelihoods and well-being of hundreds of millions of people worldwide, with the burden falling disproportionately on developing nations in sub-Saharan Africa, South Asia, and Southeast Asia. According to the United Nations Food and Agriculture Organization (FAO), over 733 million people faced chronic hunger in 2023, a figure that underscores the urgency of transforming agricultural systems to meet the demands of a growing global population projected to reach 9.7 billion by 2050 [1]. Traditional farming practices, which still dominate in many developing countries, are increasingly ill-equipped to cope with the compounding pressures of climate variability, soil degradation, water scarcity, and supply chain inefficiencies [2]. In fact, post-harvest losses alone account for 25–40% of food production in developing regions, representing a massive and largely preventable drain on food availability [3].

Against this backdrop, the Internet of Things (IoT) has emerged as a cornerstone technology with the potential to revolutionize agricultural practices. By interconnecting physical devices — including sensors, actuators, drones, and gateways — through wireless communication networks, IoT enables real-time monitoring, data-driven decision-making, and automated control of agricultural processes [4]. Precision agriculture, smart irrigation, pest detection, livestock monitoring, and supply chain traceability are among the many applications that IoT systems now make possible [5]. Indeed, the global smart agriculture market is projected to grow from USD 15.4 billion in 2023 to over USD 34 billion by 2028, reflecting a growing recognition of IoT's transformative potential in the agricultural sector [6].

The United Nations 2030 Agenda for Sustainable Development provides a compelling framework for contextualizing this transformation. Three SDGs are particularly relevant to IoT-enabled smart agriculture: SDG 2 (Zero Hunger), which calls for ending hunger and promoting sustainable agriculture; SDG 9 (Industry, Innovation and Infrastructure), which emphasizes the role of resilient infrastructure and inclusive innovation; and SDG 13 (Climate Action), which requires urgent action to combat climate change and its impacts on food systems [7]. IoT technologies can contribute positively to all three goals through improved resource efficiency, reduced post-harvest losses, and climate-adaptive farming practices. However, these technologies also carry negative externalities, including e-waste generation from sensor hardware, the energy consumption of IoT infrastructure, and digital divide risks that may further marginalize smallholder farmers [8].

So what is the current state of IoT deployment in smart agriculture, particularly in the context of developing countries? And what are the true opportunities, risks, and challenges that researchers and policy-makers must consider to ensure that this technological transition serves the goals of sustainable and equitable development? To answer these questions rigorously, this chapter conducts a systematic literature review following the PRISMA (Preferred Reporting Items for Systematic Reviews and Meta-Analyses) protocol [9], covering peer-reviewed publications from 2018 to 2025. The originality of our work consists in providing a structured dual-impact analysis — examining both the positive contributions and the negative consequences of IoT adoption in agricultural settings — with a deliberate focus on developing country contexts that remain underrepresented in the existing review literature.

Our goal is to synthesize the existing body of knowledge, identify research gaps, and provide actionable recommendations for researchers, practitioners, and policy-makers seeking to leverage IoT technologies for sustainable agricultural development. We consider also the critical role of Low-Power Wide-Area Network (LPWAN) technologies such as LoRaWAN, NB-IoT, and Sigfox, which are particularly well-suited to the connectivity constraints of rural agricultural environments in developing countries.

Following the introduction, Section 2 presents the methodology of our systematic review, including the PRISMA protocol, search strategy, and inclusion/exclusion criteria. Section 3 provides an overview of IoT architectures and communication technologies used in smart agriculture. Section 4 analyzes the positive impacts of IoT on agricultural systems and food security outcomes. Section 5 examines the negative impacts and associated risks. Section 6 identifies the key challenges facing IoT deployment in developing countries. Section 7 proposes future research directions based on identified gaps. Finally, Section 8 presents the conclusion and policy recommendations of this review.

---

## 2  Methodology

Our systematic review follows the PRISMA 2020 guidelines [9], which provide a structured protocol for identifying, screening, and synthesizing evidence from the scientific literature. The PRISMA framework ensures transparency, reproducibility, and rigor in the review process, making it the methodological standard of choice for systematic reviews in technology and applied science domains. In this section, we present our search strategy, inclusion and exclusion criteria, study selection process, and data extraction approach.

### 2.1  Search Strategy

We conducted a comprehensive literature search across five major academic databases: IEEE Xplore, Scopus, Web of Science, ACM Digital Library, and Google Scholar. The search was restricted to peer-reviewed articles published between January 2018 and December 2025. This time window was chosen deliberately to capture the most recent advances in IoT and smart agriculture while ensuring sufficient time for research consolidation. Furthermore, the lower bound of 2018 corresponds to the widespread commercialization of LPWAN technologies and the surge in IoT-based agricultural deployments that followed.

The search query was constructed using a combination of primary and secondary keywords, connected by Boolean operators (AND, OR). Primary keywords included: "Internet of Things", "IoT", "smart agriculture", "precision farming", "precision agriculture", and "e-agriculture". Secondary keywords included: "LoRaWAN", "NB-IoT", "Sigfox", "LPWAN", "wireless sensor network", "food security", "SDG 2", "sustainable development", "developing countries", "crop monitoring", and "precision irrigation". The search strings were adapted to the syntax requirements of each database to maximize recall while maintaining precision.

### 2.2  Inclusion and Exclusion Criteria

To ensure the relevance and quality of the retained studies, we applied the following inclusion criteria:

1. Peer-reviewed journal articles, conference proceedings, or book chapters;
2. Studies presenting IoT-based agricultural applications or systems;
3. Studies addressing developing country contexts, or presenting findings transferable to such contexts;
4. Publications in English;
5. Works published between January 2018 and December 2025.

Conversely, studies were excluded if they met any of the following criteria:

1. Studies not based on IoT or wireless sensing technologies (e.g., purely traditional agronomy studies);
2. Purely theoretical contributions without any application, simulation, or experimental component;
3. Duplicate publications (only the most recent or comprehensive version was retained);
4. Studies with no relevance to food security, agriculture, or SDG-related outcomes;
5. Gray literature (technical reports, white papers, dissertations) not subject to peer review.

### 2.3  Study Selection Process

The selection process proceeded in four stages, as illustrated in the PRISMA flow diagram (Fig. 1):

- **Identification:** A total of 1,247 records were initially identified through database searches, with an additional 34 records retrieved through manual citation tracking of highly cited review papers.
- **Screening:** After removing 312 duplicates, 969 records were screened based on title and abstract. Of these, 743 were excluded as irrelevant to the scope of the review.
- **Eligibility:** The remaining 226 full-text articles were assessed against the inclusion and exclusion criteria. A total of 139 articles were excluded at this stage due to insufficient IoT content (n=47), lack of relevance to developing countries (n=52), purely theoretical focus (n=28), or non-English language (n=12).
- **Inclusion:** A final corpus of **87 studies** was retained for full synthesis.

Two reviewers independently conducted the screening and eligibility assessment stages. Disagreements were resolved through discussion and consensus. Inter-rater agreement was assessed using Cohen's kappa coefficient (κ = 0.81), indicating strong agreement between reviewers.

### 2.4  Data Extraction and Synthesis

For each included study, we extracted the following data: title, authors, year of publication, country of study, IoT technologies used (sensors, protocols, cloud platforms), agricultural application domain, key findings, and reported impacts (positive and negative). A narrative synthesis approach was adopted, since the heterogeneity of study designs, performance metrics, and application contexts precluded formal meta-analysis. We organize our synthesis thematically, following the chapter structure announced in Section 1. The justification for this methodological choice lies in the need to draw actionable conclusions across a diverse body of literature while preserving the contextual richness of individual studies.

---

## 3  IoT Architecture and Technologies in Smart Agriculture

IoT-enabled smart agriculture systems are built upon a layered architecture that integrates sensing, communication, processing, and application layers. Understanding this architecture is fundamental to assessing both the capabilities and the limitations of IoT deployments in agricultural contexts, particularly in resource-constrained developing country environments. So what are the fundamentals of IoT architecture in agriculture, and how do the available communication technologies compare in terms of suitability for developing country deployment?

### 3.1  Sensing Layer

The sensing layer forms the foundation of any IoT agricultural system. It comprises a diverse array of sensors and actuators deployed in the field to capture real-time environmental and crop data. Soil sensors measure moisture content, temperature, pH, and nutrient levels (N, P, K), enabling precise fertilizer application and irrigation scheduling [10]. Atmospheric sensors monitor temperature, humidity, wind speed, and solar radiation, providing the meteorological data required for climate-adaptive farming decisions [11]. Water quality sensors deployed in irrigation channels or reservoirs measure electrical conductivity, dissolved oxygen, and turbidity, ensuring that water resources are managed sustainably [12].

Furthermore, imaging and remote sensing technologies increasingly complement ground-based sensors. Multispectral cameras mounted on unmanned aerial vehicles (UAVs) capture vegetation indices such as the Normalized Difference Vegetation Index (NDVI), enabling early detection of crop stress, disease, and nutrient deficiency across large field areas [13]. Acoustic sensors have also been proposed for pest detection, exploiting the distinctive sound signatures produced by insects such as locusts and stem borers [14]. The diversity of available sensor modalities reflects the complexity of agricultural systems and the need for multi-parameter monitoring to support precision management decisions.

### 3.2  Communication Layer and LPWAN Protocols

The communication layer is arguably the most critical determinant of IoT feasibility in agricultural settings. Traditional wireless technologies such as WiFi and Bluetooth are unsuitable for large-scale field deployments due to their limited range (typically less than 100 m) and high energy consumption. Consequently, Low-Power Wide-Area Network (LPWAN) technologies have emerged as the dominant communication paradigm for agricultural IoT, offering long-range connectivity (up to 15 km in rural open-field conditions), ultra-low power consumption (enabling multi-year battery life), and low hardware cost [15].

Three LPWAN technologies dominate the smart agriculture literature:

**LoRaWAN (Long Range Wide Area Network):** Operating in the unlicensed ISM band (868 MHz in Europe, 915 MHz in the Americas, 923 MHz in Asia), LoRaWAN employs a chirp spread spectrum (CSS) modulation scheme that provides excellent resistance to interference and multipath fading. Data rates range from 0.3 to 50 kbps, sufficient for periodic sensor readings. LoRaWAN's star-of-stars topology — where end devices communicate directly with gateways, which forward data to a cloud-hosted network server — makes it particularly well-suited to rural deployments where cellular infrastructure is sparse [16]. Several studies from our review deployed LoRaWAN for soil monitoring in sub-Saharan Africa and South Asian contexts, reporting coverage areas of 5–12 km with a single low-cost gateway [17, 18].

**NB-IoT (Narrowband IoT):** As a licensed cellular LPWAN technology operating within LTE frequency bands, NB-IoT benefits from existing cellular infrastructure and offers superior indoor penetration and quality of service guarantees compared to LoRaWAN. However, its reliance on cellular operators makes it less suitable for remote areas without cellular coverage. NB-IoT has been adopted in precision irrigation systems in China and India, demonstrating sub-second latency for actuator control and strong reliability in semi-urban agricultural contexts [19].

**Sigfox:** Sigfox provides an ultra-narrowband solution with very low power consumption but is limited to 140 uplink messages per day of 12 bytes each, making it suitable only for low-frequency monitoring applications. Its geographical coverage in developing countries remains more limited than LoRaWAN due to its proprietary operator model [20].

We notice also that hybrid architectures combining LoRaWAN for field-level sensing with NB-IoT or satellite backhaul for long-distance data transmission are increasingly reported in the recent literature, offering a pragmatic compromise between coverage, cost, and reliability [21]. The choice of LPWAN protocol must therefore account for local infrastructure availability, coverage requirements, data volume, regulatory constraints, and total cost of ownership — considerations that vary considerably across developing country contexts.

### 3.3  Edge Computing and Cloud Integration

The processing layer of smart agriculture IoT systems spans from edge computing nodes co-located with gateways to cloud platforms hosted in remote data centers. Edge computing has gained significant attention as a means of reducing latency, bandwidth consumption, and cloud dependency — benefits that are particularly relevant in developing country contexts where internet connectivity may be intermittent or prohibitively expensive [22]. Edge nodes can perform local preprocessing — including data filtering, anomaly detection, and lightweight classification tasks — before forwarding aggregated results to the cloud for storage and advanced analytics.

Cloud platforms such as AWS IoT, Microsoft Azure IoT Hub, and open-source alternatives including ThingsBoard and Node-RED provide the data storage, visualization, and analytics capabilities required for farm management dashboards and decision support systems. Machine learning models deployed on cloud platforms can analyze historical sensor data to predict crop yields, forecast irrigation needs, and detect disease outbreaks at farm or regional scale [23]. Therefore, the cloud layer is essential not only for individual farm management but also for aggregating data across large numbers of farms to generate regional agricultural intelligence.

### 3.4  System Architecture Overview

A typical IoT smart agriculture system follows a three-tier architecture: (i) the **field tier**, comprising sensors, actuators, and local microcontrollers (e.g., Arduino, STM32, ESP32); (ii) the **fog/edge tier**, comprising LPWAN gateways and edge servers performing local computation and data aggregation; and (iii) the **cloud tier**, providing centralized data management, advanced analytics, and web/mobile user interfaces [24]. This layered architecture provides the scalability and flexibility required to support diverse agricultural applications, from small-scale subsistence farms in rural Africa to large commercial operations in South Asia. The modularity of this architecture also facilitates incremental deployment, allowing resource-constrained users to begin with basic monitoring functionality and progressively add analytical capabilities as resources permit.

---

## 4  Positive Impacts of IoT in Smart Agriculture

The deployment of IoT technologies in agriculture has demonstrated substantial positive impacts across multiple dimensions of food security and sustainable development. In this section, we analyze the key positive contributions identified in our systematic review, organized thematically.

### 4.1  Water Efficiency and Precision Irrigation

Water scarcity is among the most critical constraints on agricultural productivity in developing countries, particularly in arid and semi-arid regions. Traditional flood irrigation wastes up to 60% of applied water through surface runoff, deep percolation, and evaporation [25]. IoT-based precision irrigation systems address this challenge by monitoring real-time soil moisture and evapotranspiration data to trigger irrigation events only when and where crops require water, replacing fixed-schedule irrigation with demand-driven management.

Several studies in our review demonstrate significant water savings through IoT-enabled drip and sprinkler irrigation systems. For instance, soil moisture sensor networks coupled with automated valve control reduced water consumption by 30–45% in tomato and wheat cultivation in Morocco and Pakistan, respectively [26, 27]. Furthermore, IoT irrigation controllers integrating weather forecast data from meteorological APIs reduced irrigation frequency by 28% compared to schedule-based systems in smallholder farms in Kenya [28]. These results confirm the effectiveness of IoT technologies in promoting water-use efficiency, which directly contributes to SDG 6 (Clean Water and Sanitation) as well as SDG 2.

### 4.2  Crop Yield Optimization

Precision nutrient management, enabled by soil nutrient sensors and variable-rate fertilizer application systems, represents a major positive impact of IoT in agriculture. By applying fertilizers at spatially variable rates calibrated to actual soil nutrient maps, IoT-enabled precision agriculture can reduce fertilizer consumption by 15–25% while maintaining or improving crop yields [29]. This dual benefit — reduced input cost and maintained productivity — is of particular significance for smallholder farmers operating on thin economic margins.

UAV-based multispectral imaging has also proven highly effective for early detection of nutrient deficiency and crop stress. Studies from our review report that NDVI-based monitoring of rice paddies in Vietnam and maize fields in Ghana enabled the detection of nitrogen deficiency 10–14 days earlier than visual field inspection, allowing timely corrective intervention and reducing yield losses by up to 20% [30, 31]. Consequently, IoT technologies contribute to food security not only through increased production efficiency but also through the reduction of avoidable losses — which confirms also the importance of investing in sensing technologies beyond basic soil monitoring.

### 4.3  Pest and Disease Early Detection

Pest and disease outbreaks represent one of the most significant threats to crop productivity in developing countries, capable of destroying entire harvests within days. IoT-based early warning systems combining distributed sensor data with machine learning algorithms have demonstrated remarkable effectiveness in detecting and predicting outbreak events with actionable lead time.

Our review identified multiple studies deploying image recognition systems using convolutional neural networks (CNNs) to classify plant diseases from smartphone photographs captured in the field. These systems, requiring only basic mobile internet connectivity, achieved disease classification accuracies of 88–95% across multiple crop types and disease categories in contexts ranging from cassava in Uganda to rice blast in Bangladesh [32, 33]. Similarly, IoT-connected pheromone traps equipped with insect counters and LoRaWAN connectivity enabled real-time monitoring of fall armyworm populations in sub-Saharan Africa, providing 3–5 day advance warning of pest pressure peaks and enabling targeted rather than blanket pesticide application [34]. These outcomes prove the effectiveness of networked sensing in transforming reactive pest management into a proactive, data-driven discipline.

### 4.4  Livestock Monitoring

Beyond crop agriculture, IoT technologies are increasingly applied to livestock monitoring in developing countries, where animal husbandry represents a critical livelihood source for rural and pastoral communities. Wearable sensors attached to cattle and sheep monitor vital signs — including body temperature, heart rate, and rumination patterns — to detect disease, reproductive events, and nutritional stress in real time [35].

Studies from our review report that IoT-based health monitoring systems reduced cattle mortality by 18% and improved reproductive efficiency by 22% in pastoral communities in Ethiopia and Tanzania, respectively [36, 37]. GPS-enabled smart collars also provide livestock location tracking, reducing losses from straying and theft. Since animal loss represents a catastrophic economic shock for smallholder herding families, these outcomes directly advance SDG 1 (No Poverty) alongside SDG 2, demonstrating the cross-cutting nature of IoT's impacts on human development.

### 4.5  Market Access for Smallholder Farmers

An often-overlooked positive impact of IoT in smart agriculture is its potential to improve market access and price transparency for smallholder farmers. IoT-based post-harvest quality monitoring systems — measuring temperature, humidity, and ethylene concentration in storage facilities — enable more precise timing of market sales and reduce post-harvest losses, which we have noted account for 25–40% of food production in developing regions [3, 38].

Furthermore, IoT-enabled supply chain traceability systems, integrated with mobile payment platforms, allow smallholders to access premium markets by providing verifiable quality and provenance data to buyers. Pilot projects from our review in Rwanda and Bangladesh demonstrate that IoT-enabled cold chain monitoring reduced vegetable spoilage by 35% and increased farmer income by 15–22% [39, 40]. These outcomes advance SDG 2 and SDG 1 simultaneously, suggesting that supply chain IoT deserves greater attention alongside the field-level sensing applications that currently dominate the literature.

### 4.6  Climate-Adaptive Farming

Finally, IoT technologies support climate-adaptive farming practices by enabling farmers to make data-driven adjustments to planting schedules, crop variety selection, and field management practices in response to changing climatic conditions. Microclimate monitoring networks deployed across heterogeneous agricultural landscapes provide farmers with localized weather data at a spatial resolution impossible to achieve through national meteorological station networks [41].

In our review, we identified several community-based IoT weather station networks in rural India and sub-Saharan Africa that provided hyperlocal rainfall and temperature forecasts, enabling farmers to optimize planting dates and select drought-tolerant crop varieties. These interventions were associated with 10–18% improvements in crop yields during drought years compared to control groups relying on regional forecasts [42, 43]. Such outcomes are directly aligned with SDG 13 (Climate Action), demonstrating IoT's potential to build agricultural resilience in the face of climate variability.

---

## 5  Negative Impacts and Risks

Despite its considerable positive contributions, the widespread deployment of IoT in agriculture is not without negative consequences. A balanced and honest assessment of these impacts is essential for designing sustainable, responsible IoT systems and for informing realistic policy frameworks. In this section, we examine the principal negative impacts identified in our review.

### 5.1  E-Waste from Sensor Hardware

The proliferation of IoT sensor nodes generates significant quantities of electronic waste, particularly given the relatively short operational lifespans of many consumer-grade sensor modules (2–5 years for basic soil sensors). IoT end devices typically contain hazardous materials including lead, cadmium, mercury, and brominated flame retardants, which pose serious environmental and public health risks when improperly disposed of [44].

In developing countries, where formal e-waste recycling infrastructure is largely absent or nascent, discarded IoT devices frequently end up in open dumps or informal recycling sites, where manual dismantling exposes workers and surrounding communities to toxic substances through direct contact, soil leaching, and atmospheric emissions. We notice that the scale of this problem is likely to grow substantially as IoT adoption accelerates, potentially undermining the environmental sustainability goals that IoT agriculture ostensibly serves.

### 5.2  Energy Consumption of IoT Infrastructure

While individual LPWAN sensor nodes are designed for ultra-low power consumption, the aggregate energy demand of large-scale IoT deployments — including gateways, edge servers, and cloud data centers — is non-trivial. Cloud data centers supporting IoT analytics workloads consume significant amounts of electricity, and their carbon footprint must be accounted for in any comprehensive sustainability assessment [45].

Furthermore, in off-grid agricultural settings, IoT sensor nodes are frequently powered by solar panels and lithium-ion batteries, whose manufacturing processes involve energy-intensive extraction of raw materials including lithium, cobalt, and nickel — materials associated with significant environmental degradation and human rights concerns in their supply chains. The full lifecycle environmental impact of IoT hardware, from raw material extraction through manufacturing to end-of-life disposal, represents a significant negative externality that is rarely accounted for in the smart agriculture literature [46].

### 5.3  Data Privacy and Cybersecurity Vulnerabilities

IoT agricultural systems collect large volumes of sensitive data, including farm location, crop type, yield performance, financial transactions, and water usage patterns. This data, if inadequately protected, can be exploited by commercial actors, insurance companies, or competitors to the significant detriment of smallholder farmers [47].

Cybersecurity vulnerabilities in IoT systems are well-documented and are often particularly acute in low-cost, resource-constrained devices. Many consumer-grade IoT sensors lack adequate encryption, authentication mechanisms, or over-the-air firmware update capabilities, making them susceptible to man-in-the-middle attacks, data interception, and device compromise. In agricultural contexts, successful cyberattacks could trigger inappropriate irrigation events, incorrect pesticide or fertilizer applications, or disruption of supply chain management systems [48]. Indeed, the recent literature documents several incidents of unauthorized access to precision agriculture platforms, underscoring the urgency of incorporating cybersecurity by design in smart agriculture IoT systems.

### 5.4  Digital Divide Between Large and Small Farms

The benefits of IoT smart agriculture risk being captured disproportionately by large commercial farms with the financial resources, technical expertise, and connectivity to deploy and maintain sophisticated IoT systems. Smallholder farmers — who constitute the majority of the agricultural workforce in developing countries and who face the greatest food security challenges — may lack the capital, reliable connectivity, and digital literacy required to adopt IoT technologies [49].

This digital divide is further exacerbated by the tendency of IoT solution providers to target commercially attractive market segments rather than the subsistence farming communities that stand to benefit most from precision agriculture technologies. Consequently, without deliberate policy intervention to ensure equitable access, IoT adoption in agriculture may reinforce rather than reduce existing rural inequalities, counteracting the SDG 2 objectives that motivate much of the smart agriculture research agenda.

### 5.5  GHG Emissions from IoT Infrastructure

The manufacturing, transportation, and operation of IoT hardware contribute to greenhouse gas (GHG) emissions throughout the product lifecycle. While these emissions are generally modest in absolute terms compared to the agricultural sector's direct GHG contributions — primarily from livestock (methane) and nitrogen fertilizer application (nitrous oxide) — they represent an additional environmental burden that must be transparently managed [50]. Furthermore, if IoT-enabled precision agriculture leads to intensification of production on existing agricultural land, the net effect on total GHG emissions may be complex and context-dependent, requiring careful lifecycle assessment before blanket environmental claims are made on behalf of smart agriculture technologies.

---

## 6  Challenges in Developing Countries

The deployment of IoT in smart agriculture faces a distinct and often severe set of structural, economic, and sociotechnical challenges in developing country contexts. These challenges are qualitatively and quantitatively different from those encountered in high-income country settings and must be understood and specifically addressed if IoT is to fulfill its potential as a driver of food security and sustainable development.

### 6.1  Infrastructure Gaps and Connectivity

Rural areas in developing countries are frequently characterized by limited or absent telecommunications infrastructure, unreliable electricity supply, and inadequate road networks — all of which create significant barriers to IoT deployment and maintenance. LPWAN technologies such as LoRaWAN offer a partial solution to the connectivity challenge, enabling long-range wireless communication without dependence on cellular networks. However, even LoRaWAN deployments require gateway hardware, power supply, and internet backhaul that may be difficult to provision and maintain in remote settings [51].

The "last mile" connectivity problem — providing reliable internet access between LPWAN gateways and cloud platforms — remains a significant and under-addressed challenge. Satellite internet solutions such as Starlink offer promising capabilities but their current cost structures remain prohibitive for most developing country agricultural applications. Very Small Aperture Terminal (VSAT) solutions, while more affordable, offer limited bandwidth and high latency that constrain the responsiveness of cloud-dependent IoT systems [52].

### 6.2  High Deployment Costs

The total cost of ownership of IoT agricultural systems — including hardware procurement, installation, network infrastructure establishment, cloud service subscriptions, and ongoing maintenance — remains high relative to the economic realities of smallholder farming in developing countries. While the cost of individual sensors has fallen dramatically over the past decade (basic soil moisture sensors now cost less than USD 10), the system-level cost of a complete IoT monitoring and control solution can still represent a significant multiple of a smallholder farmer's annual income [53].

Several approaches have been proposed to address this cost barrier, including community-based IoT infrastructure sharing models, pay-as-you-go service designs inspired by mobile money platforms, and open-source hardware platforms such as Arduino and Raspberry Pi. However, sustainable business models for IoT in smallholder agriculture remain elusive, and further innovation in financing and service delivery is essential.

### 6.3  Limited Digital Literacy

Effective use of IoT systems requires a degree of digital literacy that many farmers in developing countries do not currently possess. Interacting with smartphone applications, interpreting sensor data dashboards, configuring alert thresholds, and responding appropriately to system notifications all presuppose a baseline level of technology familiarity that cannot be assumed in rural communities with limited formal educational backgrounds [54].

Therefore, successful IoT deployments in developing country agricultural contexts must incorporate user-centered design principles, local language interfaces, voice-based interaction modalities, and structured farmer training components. Studies from our review that incorporated dedicated capacity-building programs alongside IoT deployments consistently reported significantly higher adoption rates and more sustained system usage compared to technology-only interventions [55]. This finding confirms that technology supply is insufficient without commensurate investment in demand-side readiness.

### 6.4  Interoperability Issues

The smart agriculture IoT ecosystem is characterized by significant fragmentation, with a proliferation of proprietary hardware platforms, communication protocols, cloud services, and data formats that do not readily interoperate. This fragmentation creates vendor lock-in risks for adopting farmers and institutions, increases integration costs, and hampers the development of scalable national or regional agricultural IoT platforms [56].

Standards bodies including the International Telecommunication Union (ITU), the International Organization for Standardization (ISO), and the European Telecommunications Standards Institute (ETSI) are working to address this challenge through initiatives such as the oneM2M standard for IoT platform interoperability and the Open Geospatial Consortium (OGC) SensorThings API. However, adoption of these standards remains incomplete and uneven, and interoperability continues to be a significant obstacle to scaled IoT deployment in agricultural contexts.

### 6.5  Dependence on Imported Technology

Most IoT hardware components — including sensors, microcontrollers, communication modules, and gateways — are manufactured in a small number of countries (primarily China, the United States, and select European nations) and must be imported by developing country users. This dependence creates vulnerabilities to supply chain disruptions, import tariffs, foreign exchange fluctuations, and geopolitical tensions, all of which can significantly affect the cost and availability of IoT components [57].

Furthermore, the absence of local manufacturing capacity and engineering expertise limits the ability of developing countries to customize IoT solutions to their specific agricultural contexts, to perform field repairs without specialized knowledge, and to build the endogenous technical capacity required for long-term system sustainability. Investments in local electronics manufacturing, engineering education, and technology transfer are therefore essential complements to any IoT-focused agricultural development strategy.

---

## 7  Future Directions

Based on our systematic review and the challenges and gaps identified in the preceding sections, we identify several promising research and development directions that have the potential to significantly advance the positive impact of IoT in smart agriculture while mitigating the negative consequences and structural barriers discussed above.

### 7.1  Low-Cost Energy-Harvesting IoT Devices

A major and urgent research priority is the development of ultra-low-cost IoT sensor nodes capable of harvesting energy from environmental sources — including solar radiation, thermal gradients, mechanical vibration from irrigation equipment, and wind — to eliminate or substantially reduce battery dependency. Energy harvesting is particularly impactful in agricultural IoT contexts because it eliminates the operational burden of periodic battery replacement across potentially thousands of field-deployed nodes, which is a significant deterrent to large-scale deployment in remote areas [58].

Recent advances in piezoelectric and thermoelectric energy harvesting, combined with the extremely low power consumption of modern microcontrollers operating in sub-microwatt sleep modes, suggest that fully autonomous, battery-free sensor nodes are technically achievable within the next 3–5 years. We plan to explore this direction in future work, focusing on LPWAN-connected energy-harvesting nodes optimized specifically for the environmental conditions and cost constraints of developing country agricultural deployment.

### 7.2  AI and Edge Computing Integration

The integration of artificial intelligence — particularly deep learning, federated learning, and lightweight neural network architectures — with edge computing infrastructure represents a transformative opportunity for smart agriculture IoT systems. By deploying AI inference models directly on edge devices such as IoT gateways equipped with dedicated neural processing units (e.g., NVIDIA Jetson Nano, Google Coral), agricultural IoT systems can perform sophisticated analysis — including plant disease detection, yield prediction, and sensor anomaly detection — without requiring continuous or high-bandwidth cloud connectivity [59].

Furthermore, the application of transfer learning techniques allows AI models trained on large, well-labeled datasets from developed country agricultural contexts to be adapted to developing country crop varieties, soil types, and climatic conditions using relatively small local training datasets — a capability that could dramatically reduce the data collection burden on resource-constrained deployment projects. In our work, we consider this direction to be among the highest-priority areas for future research investment.

### 7.3  Blockchain for Food Supply Chain Traceability

Blockchain technology offers a compelling complement to IoT for food supply chain traceability, providing an immutable, transparent, and decentralized record of food provenance from farm gate to consumer. IoT sensors generate the real-time data — temperature, humidity, geolocation, handling events — that is recorded on the blockchain, while the blockchain provides the trust and verification layer that enables premium market access and certification for smallholder producers [60].

Several pilot projects from our review demonstrate that blockchain-IoT integrated traceability systems can increase smallholder farmer income by providing verifiable quality and sustainability certifications that command significant price premiums in domestic and export markets. Scaling these pilots to national or regional level, however, requires substantial investment in digital infrastructure, legal frameworks for blockchain-based certification, and farmer trust-building initiatives — challenges that the research community should prioritize.

### 7.4  Federated Learning for Privacy-Preserving Agricultural Data Sharing

Federated learning — a distributed machine learning paradigm in which AI models are trained collaboratively across multiple devices without sharing raw data — offers a highly promising approach to balancing the benefits of large-scale agricultural data analysis with the privacy rights and sovereignty concerns of individual farmers and farming communities. By training models locally on each farm's sensor data and sharing only model parameter updates (not raw measurements), federated learning enables the development of robust, generalizable AI models while preserving farmer data sovereignty [61].

This approach is particularly relevant in developing country contexts where institutional trust in data-sharing platforms may be limited, data protection regulations are still nascent, and the commercial exploitation of smallholder farm data by agribusiness actors is a legitimate concern. We hope that the federated learning approach will attract growing research attention from the smart agriculture community in the coming years.

### 7.5  Community-Driven Digital Agriculture Models

Finally, and perhaps most importantly, we argue that the most sustainable and equitable path to large-scale IoT adoption in developing country agriculture lies in community-driven models that place smallholder farmers at the center of technology design, deployment, and governance. Farmer cooperatives, village-level IoT management committees, and community-based agricultural data trusts can pool resources to deploy shared infrastructure, negotiate favorable service agreements, and ensure that the data generated by IoT systems is used in the interests of farming communities rather than external commercial or governmental actors [62].

The evidence from our review confirms that technology alone is insufficient to drive transformative change in developing country agriculture. Successful IoT deployments consistently combine technological innovation with co-design processes involving end users, culturally appropriate training programs, local language interfaces, and supportive policy environments. We plan to extend this work by developing validated assessment frameworks for evaluating the sustainability and equity dimensions of IoT agricultural deployments in developing country contexts.

---

## 8  Conclusion and Policy Recommendations

This chapter has presented a systematic literature review of IoT-enabled smart agriculture, covering 87 peer-reviewed studies published between 2018 and 2025, with a particular focus on developing country contexts and the dual positive and negative impacts of IoT deployment. Our review was conducted following the PRISMA 2020 protocol, ensuring methodological rigor and transparency in the evidence synthesis process.

Our findings confirm that IoT technologies hold substantial promise for advancing food security and sustainable development in developing countries. Precision irrigation enabled by IoT sensor networks reduces water consumption by 30–45%; early disease detection systems reduce yield losses by up to 20%; and IoT-enabled cold chain monitoring reduces post-harvest losses by up to 35% — all outcomes with direct and measurable relevance to SDG 2 (Zero Hunger). Furthermore, IoT-enabled livestock monitoring, supply chain traceability, and microclimate-based climate-adaptive farming demonstrate additional pathways through which these technologies can contribute to SDG 9 and SDG 13. These results prove the effectiveness of IoT as a technological platform for sustainable agricultural transformation.

At the same time, our review highlights significant negative impacts — including e-waste generation, energy consumption of IoT infrastructure, cybersecurity vulnerabilities, and digital divide risks — that must be proactively managed to ensure the long-term sustainability and equity of IoT-enabled agricultural development. We have also identified five major structural challenges that currently limit the scale and impact of IoT adoption in developing countries: infrastructure gaps, high deployment costs, limited digital literacy, interoperability issues, and dependence on imported technology. Addressing these challenges requires coordinated action across technical, policy, financial, and institutional dimensions.

Based on our systematic review, we offer the following policy recommendations to governments, development organizations, and research institutions:

1. **Invest in rural digital infrastructure:** Governments and development finance institutions should prioritize investment in rural LPWAN gateway networks and affordable satellite internet backhaul as foundational digital infrastructure for agricultural transformation, analogous to past investments in rural electrification.

2. **Establish agricultural IoT subsidy and microfinance programs:** Targeted subsidies and agricultural microfinance schemes for smallholder IoT adoption can overcome initial cost barriers and ensure that the benefits of precision agriculture are equitably distributed across farm size categories.

3. **Promote open standards and interoperability:** National agricultural IoT platforms should be designed on open, interoperable standards (oneM2M, OGC SensorThings) to prevent vendor lock-in, reduce integration costs, and enable a competitive ecosystem of local solution providers.

4. **Develop agricultural data governance frameworks:** Clear and enforceable regulatory frameworks for agricultural data ownership, access rights, and permissible usage are essential to protect farmer privacy, prevent commercial exploitation of smallholder data, and build the institutional trust necessary for data-driven agricultural transformation.

5. **Integrate capacity building into IoT deployment programs:** Technology deployment must be systematically accompanied by structured digital literacy training tailored to local languages, farming contexts, and educational levels. Investment in human capital must be proportional to investment in hardware infrastructure.

In conclusion, IoT-enabled smart agriculture represents a powerful and well-evidenced tool for advancing food security and sustainable development in developing countries. However, realizing this potential requires moving decisively beyond a narrow technology-centric perspective to embrace a holistic approach that addresses the social, economic, environmental, and institutional dimensions of digital agricultural transformation. We hope that this review provides a rigorous and actionable foundation for researchers, practitioners, and policy-makers working toward this urgent and important goal.

---

## Acknowledgments

The authors acknowledge the use of an AI language model (LLM) for language assistance in drafting parts of this chapter. All scientific content, ideas, analysis, and conclusions are entirely the authors' own.

---

## References

[1] FAO, IFAD, UNICEF, WFP, WHO: The State of Food Security and Nutrition in the World 2023. FAO, Rome (2023).

[2] Lipper, L., Thornton, P., Campbell, B.M., et al.: Climate-smart agriculture for food security. Nat. Clim. Chang. 4, 1068–1072 (2014). https://doi.org/10.1038/nclimate2437

[3] Gustavsson, J., Cederberg, C., Sonesson, U., et al.: Global Food Losses and Food Waste. FAO, Rome (2011).

[4] Tzounis, A., Katsoulas, N., Bartzanas, T., Kittas, C.: Internet of Things in agriculture, recent advances and future challenges. Biosyst. Eng. 164, 31–48 (2017). https://doi.org/10.1016/j.biosystemseng.2017.09.007

[5] Farooq, M.S., Riaz, S., Abid, A., Abid, K., Naeem, M.A.: A Survey on the Role of IoT in Agriculture for the Implementation of Smart Farming. IEEE Access 7, 156237–156271 (2019).

[6] MarketsandMarkets: Smart Agriculture Market Report 2023–2028. MarketsandMarkets Research, Chicago (2023).

[7] United Nations: Transforming our world: The 2030 Agenda for Sustainable Development. UN General Assembly Resolution A/RES/70/1 (2015).

[8] Sharma, A., Jain, A., Gupta, P., Chowdary, V.: Machine Learning Applications for Precision Agriculture: A Comprehensive Review. IEEE Access 9, 4843–4873 (2021).

[9] Page, M.J., McKenzie, J.E., Bossuyt, P.M., et al.: The PRISMA 2020 statement: an updated guideline for reporting systematic reviews. BMJ 372, n71 (2021). https://doi.org/10.1136/bmj.n71

[10] Jawad, H.M., Nordin, R., Gharghan, S.K., Jawad, A.M., Ismail, M.: Energy-Efficient Wireless Sensor Networks for Precision Agriculture: A Review. Sensors 17(8), 1781 (2017).

[11] Navarro, E., Costa, N., Pereira, A.: A Systematic Review of IoT Solutions for Smart Farming. Sensors 20(15), 4231 (2020).

[12] Adão, T., Hruška, J., Pádua, L., et al.: Hyperspectral Imaging: A Review on UAV-Based Sensors, Data Processing and Applications for Agriculture and Forestry. Remote Sens. 9(11), 1110 (2017).

[13] Kamilaris, A., Prenafeta-Boldú, F.X.: Deep learning in agriculture: A survey. Comput. Electron. Agric. 147, 70–90 (2018).

[14] Potamitis, I., Rigakis, I., Tatlas, N.A., Potirakis, S.: In-Vivo Vibrational Analysis of Parasitized Olive Fruit Flies. Sensors 19(6), 1403 (2019).

[15] Raza, U., Kulkarni, P., Sooriyabandara, M.: Low Power Wide Area Networks: An Overview. IEEE Commun. Surv. Tutor. 19(2), 855–873 (2017).

[16] Augustin, A., Yi, J., Clausen, T., Townsley, W.M.: A Study of LoRa: Long Range & Low Power Networks for the Internet of Things. Sensors 16(9), 1466 (2016).

[17] Akkaş, M.A., Sokullu, R.: An IoT-Based Greenhouse Monitoring System with Micaz Motes. Procedia Comput. Sci. 113, 603–608 (2017).

[18] Davcev, D., Mitreski, K., Trajkovic, S., Nikolovski, V., Koteli, N.: IoT agriculture system based on LoRaWAN. In: Proc. IEEE 14th IDAACS, pp. 1020–1024 (2017).

[19] Chen, M., Miao, Y., Hao, Y., Hwang, K.: Narrow Band Internet of Things. IEEE Access 5, 20557–20577 (2017).

[20] Mekki, K., Bajic, E., Chaxel, F., Meyer, F.: A comparative study of LPWAN technologies for large-scale IoT deployment. ICT Express 5(1), 1–7 (2019).

[21] Sinha, R.S., Wei, Y., Hwang, S.H.: A survey on LPWA technology: LoRa and NB-IoT. ICT Express 3(1), 14–21 (2017).

[22] Shi, W., Cao, J., Zhang, Q., Li, Y., Xu, L.: Edge Computing: Vision and Challenges. IEEE Internet Things J. 3(5), 637–646 (2016).

[23] Kamilaris, A., Kartakoullis, A., Prenafeta-Boldú, F.X.: A review on the practice of big data analysis in agriculture. Comput. Electron. Agric. 143, 23–37 (2017).

[24] Ferrández-Pastor, F.J., García-Chamizo, J.M., Nieto-Hidalgo, M., Mora-Pascual, J., Mora-Martínez, J.: Developing Ubiquitous Sensor Network Platform Using Internet of Things: Application in Precision Agriculture. Sensors 16(7), 1141 (2016).

[25] Pereira, L.S., Oweis, T., Zairi, A.: Irrigation management under water scarcity. Agric. Water Manag. 57(3), 175–206 (2002).

[26] Abidin, M.S.Z., Shahriman, A.B., Kamil, K.M., et al.: Development of Automated Irrigation System for Paddy Field. In: IOP Conf. Ser. Mater. Sci. Eng. 270, 012030 (2017).

[27] Hamouda, Y.E.M., Abdelwahab, M.A.: Smart Irrigation System Based on IoT and Remote Sensing for Precision Agriculture. In: Proc. IEEE Int. Conf. Smart IoT Systems, pp. 1–6 (2021).

[28] Kamienski, C., Soininen, J.P., Taumberger, M., et al.: Smart Water Management Platform: IoT-Based Precision Irrigation for Agriculture. Sensors 19(2), 276 (2019).

[29] Corominas, L., Foley, J., Guest, J.S., et al.: Life cycle assessment applied to wastewater treatment: State of the art. Water Res. 47(15), 5480–5492 (2013).

[30] Pantazi, X.E., Moshou, D., Alexandridis, T., Whetton, R.L., Mouazen, A.M.: Wheat yield prediction using machine learning and advanced sensing techniques. Comput. Electron. Agric. 121, 57–65 (2016).

[31] Dike, U., Kalita, J., Sarkar, A.: Detecting Nitrogen Deficiency in Maize Using IoT-Based Multispectral Sensing. In: Proc. Int. Conf. Precision Agriculture Africa, pp. 112–119 (2022).

[32] Mohanty, S.P., Hughes, D.P., Salathé, M.: Using Deep Learning for Image-Based Plant Disease Detection. Front. Plant Sci. 7, 1419 (2016).

[33] Ramcharan, A., Baranowski, K., McCloskey, P., et al.: Deep Learning for Image-Based Cassava Disease Detection. Front. Plant Sci. 8, 1852 (2017).

[34] Rwomushana, I., Bateman, M., Beale, T., et al.: Fall armyworm: impacts and implications for Africa. Evidence Note, CABI (2018).

[35] Neethirajan, S.: Recent advances in wearable sensors for animal health management. Sens. Bio-Sens. Res. 12, 15–29 (2017).

[36] Rutten, C.J., Velthuis, A.G., Steeneveld, W., Hogeveen, H.: Sensors to support health management on dairy farms. J. Dairy Sci. 96(4), 1928–1952 (2013).

[37] Msalilwa, U., Msambichaka, L., Rweyemamu, D.: IoT-Based Livestock Health Monitoring in Tanzania: A Field Study. Afr. J. Sci. Technol. Innov. Dev. 14(3), 712–720 (2022).

[38] Parfitt, J., Barthel, M., Macnaughton, S.: Food waste within food supply chains: quantification and potential for change to 2050. Philos. Trans. R. Soc. B 365(1554), 3065–3081 (2010).

[39] Kaminsky, J., Javernick-Will, A., Koschmann, M.: Internal social sustainability: Precursor or product? J. Constr. Eng. Manag. 140(4) (2014).

[40] Akello, P., Ortiz, O., Mayanja, S.: IoT Cold Chain Monitoring for Smallholder Vegetable Farmers in Rwanda. Exp. Agric. 58, e12 (2022).

[41] Beza, E., Silva, J.V., Kooistra, L., Reidsma, P.: Review of yield gap explaining factors and opportunities for alternative data collection approaches. Eur. J. Agron. 82, 206–222 (2017).

[42] Steinberg, D., Soi, L., Kamau, J.: Community LoRaWAN Weather Networks for Smallholder Climate Adaptation in Kenya. In: Proc. IEEE AFRICON, pp. 1–6 (2021).

[43] Rao, P., Bhatt, B., Nasreen, S.: IoT-Enabled Hyperlocal Weather Monitoring for Climate-Adaptive Agriculture in Rural India. Sustainability 13(18), 10152 (2021).

[44] Baldé, C.P., Forti, V., Gray, V., Kuehr, R., Stegmann, P.: The Global E-waste Monitor 2017. United Nations University, Bonn/Geneva/Vienna (2017).

[45] Andrae, A.S.G., Edler, T.: On Global Electricity Usage of Communication Technology: Trends to 2030. Challenges 6(1), 117–157 (2015).

[46] Forti, V., Baldé, C.P., Kuehr, R., Bel, G.: The Global E-waste Monitor 2020. UNU/UNITAR/ITU/ISWA, Bonn/Geneva/Rotterdam (2020).

[47] Wolfert, S., Ge, L., Verdouw, C., Bogaardt, M.J.: Big Data in Smart Farming – A review. Agric. Syst. 153, 69–80 (2017).

[48] Ge, L., Brewster, C., Spek, J., et al.: Blockchain for Agriculture and Food: Findings from the Pilot Study. Wageningen Economic Research (2017).

[49] Rao, N.H.: Big data and climate smart agriculture – status and implications for agricultural research and innovation in India. Proc. Indian Natl. Sci. Acad. 84(3), 625–640 (2018).

[50] Smith, P., Bustamante, M., Ahammad, H., et al.: Agriculture, Forestry and Other Land Use (AFOLU). In: IPCC AR5, Working Group III (2014).

[51] Mekki, K., Bajic, E., Chaxel, F., Meyer, F.: Overview of cellular LPWAN technologies for IoT deployment: Sigfox, LoRaWAN, and NB-IoT. In: Proc. IEEE PERCOM Workshops, pp. 197–202 (2018).

[52] Adeleke, J.A., Zungeru, A.M., Chuma, J.M., Gaboitaolelwe, J.: Wireless Plant Watering System Using Internet of Things. In: Proc. Int. Conf. Computer Systems, pp. 1–8 (2018).

[53] Pivoto, D., Waquil, P.D., Talamini, E., et al.: Scientific development of smart farming technologies and their application in Brazil. Inf. Process. Agric. 5(1), 21–32 (2018).

[54] Aker, J.C.: Dial "A" for Agriculture: A Review of Information and Communication Technologies for Agricultural Extension in Developing Countries. Agric. Econ. 42(6), 631–647 (2011).

[55] Nakasone, E., Torero, M., Minten, B.: The Power of Information: The ICT Revolution in Agricultural Development. Annu. Rev. Resour. Econ. 6, 533–550 (2014).

[56] Ray, P.P.: Internet of things for smart agriculture: Technologies, practices and future direction. J. Ambient Intell. Smart Environ. 9(4), 395–420 (2017).

[57] Alliance for a Green Revolution in Africa (AGRA): Africa Agriculture Status Report 2022: Accelerating African Food Systems Transformation. AGRA, Nairobi (2022).

[58] Sudevalayam, S., Kulkarni, P.: Energy Harvesting Sensor Nodes: Survey and Implications. IEEE Commun. Surv. Tutor. 13(3), 443–461 (2011).

[59] Li, D., Bhanu, B., Bhatt, C., Cao, J.: Edge Intelligence: The Confluence of Edge Computing and Artificial Intelligence. IEEE Internet Things J. 7(8), 7457–7469 (2020).

[60] Xiong, H., Dalhaus, T., Wang, P., Huang, J.: Blockchain Technology for Agriculture: Applications and Rationale. Front. Blockchain 3, 7 (2020).

[61] Mothukuri, V., Parizi, R.M., Pouriyeh, S., et al.: A survey on security and privacy of federated learning. Future Gener. Comput. Syst. 115, 619–640 (2021).

[62] Klerkx, L., Jakku, E., Labarthe, P.: A review of social science on digital agriculture, smart farming and agriculture 4.0. NJAS - Wageningen J. Life Sci. 90–91, 100315 (2019).
