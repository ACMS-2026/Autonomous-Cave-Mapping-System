# Autonomous-Cave-Mapping-System
Autonomous Cave Mapping System (ACMS) ist ein autonomes Drohnensystem zur Erkundung und digitalen Vermessung von Höhlen. Mithilfe von Kameras, Sensoren und KI erstellt die Drohne selbstständig Karten und 3D-Modelle schwer zugänglicher Bereiche und unterstützt so Forschung, Dokumentation und Naturschutz.

Autonomous Cave Mapping System (ACMS) is an autonomous drone system designed for the exploration and digital mapping of caves. Using cameras, sensors, and artificial intelligence (AI), the drone independently creates maps and 3D models of hard-to-reach areas, thereby supporting scientific research, documentation, and nature conservation.
1. Project Idea:

Autonomous Cave Mapping System (ACMS)

The Autonomous Cave Mapping System (ACMS) project describes an autonomous drone system designed for the exploration, surveying, and visual documentation of caves and underground structures. The goal of the system is to investigate hard-to-reach or previously unknown cave areas without human control and to generate digital maps and 3D models from the collected data.

The drone starts from a defined point either inside or at the entrance of a cave system. From there, it navigates independently through the environment, detects obstacles, and explores adjacent passages. Throughout the mission, the system continuously collects sensor data for orientation, including distance measurements, positional information, and structural data of the surrounding environment.

A central component of the system is autonomous mapping. Using suitable algorithms for Simultaneous Localization and Mapping (SLAM), the drone creates a dynamic 3D model of the cave. Dimensions such as passage width, height, and depth are automatically determined and incorporated into a digital map.

In addition, the drone captures optical data in the form of high-resolution images or video recordings of the cave walls. These recordings can later be used for the analysis of geological structures or the documentation of special features.

After completing the exploration mission or reaching predefined criteria such as a time limit or low battery level, the drone autonomously returns to its starting point. All collected data are stored and can subsequently be analyzed.

The ACMS is particularly suitable for applications in research, geology, rescue technology, and the exploration of unknown underground systems. By combining autonomous navigation, sensor fusion, and image processing, the project enables efficient and safe exploration of environments that are difficult or dangerous for humans to access.

2. Background

What Problem Does the Idea Solve?

Natural caves are among the most fascinating yet fragile geological environments on Earth. Many cave systems contain unique stalactite and stalagmite formations, mineral deposits, fossils, and other geological structures that have developed over thousands or even millions of years. These natural archives provide valuable information for geology, paleontology, climate research, and many other scientific disciplines.

Today, the exploration and documentation of such caves are often carried out by cavers who physically enter and survey the cave systems. However, this process presents several challenges. Many cave sections are difficult to access and require significant physical effort. Furthermore, every human visit may impact the fragile ecosystem and geological structures of a cave. Simply touching speleothems, walking across sensitive ground areas, or increasing visitor numbers can cause damage that remains visible for very long periods or may even be irreversible.

The planned Autonomous Cave Mapping System (ACMS) aims to reduce these issues. Its objective is the autonomous collection of image and sensor data within a cave. These data can then be used to generate a high-resolution digital 3D model. This makes it possible to document caves in great detail and provide virtual access without requiring large numbers of people to physically enter the cave.

How Widespread Is This Problem?

The described problem is not limited to individual caves but is relevant worldwide. Numerous caves are protected as natural or cultural heritage sites and can only be accessed under strict regulations. At the same time, scientists, cavers, educational institutions, and the public have a strong interest in exploring and documenting these unique environments.

Many caves are accessible only to experienced cavers. Narrow passages, steep shafts, difficult climbing sections, and long approaches prevent much of the population from visiting them directly. Even within caving organizations, age or health limitations may prevent members from actively participating in cave expeditions.

As a result, the digitalization and virtual representation of cave systems are becoming increasingly important. Modern 3D models allow scientific investigations, documentation, and public education while minimizing the impact on the actual cave environment.

Personal Motivation

My personal motivation for this project stems from my long-standing interest in technology, robotics, and autonomous systems, as well as my membership in the Kluterthöhle Working Group (AKKH). Through active involvement in cave exploration, I have gained firsthand insight into the challenges associated with the exploration, surveying, and documentation of cave systems.

It has become particularly clear that not everyone has the opportunity to explore a cave personally. Many caves require considerable physical fitness and experience. Furthermore, there are club members and interested individuals who are no longer able to participate in cave expeditions due to age or health limitations.

A digital 3D model could provide these individuals with access to the cave. Virtual representation allows users to view cave chambers, follow scientific observations, and study geological features without being physically present. This makes information and research results accessible to a much broader audience.

Reference

Author / Organization: Kluterthöhle Working Group (AKKH)
Website Title: Kluterthöhle Working Group (Official Website)
URL: https://www.akkh.de/
Date Accessed: June 14, 2026

Why Is This Topic Important and Interesting?

This topic combines several highly relevant scientific and societal aspects. On the one hand, the project contributes to the protection of sensitive natural and cultural environments by reducing the number of required cave visits. On the other hand, it supports scientific documentation and the long-term preservation of geological information.

Another important aspect is knowledge generation. Many caves were documented in the past using manual surveying methods. Data collected by an autonomous system could be compared with existing survey data, making it possible to verify measurements, identify discrepancies, or capture additional details. At the same time, digital datasets can be archived and utilized for future research projects.

Furthermore, the project integrates modern technologies from the fields of autonomous navigation, sensing, image processing, photogrammetry, and 3D modeling. It demonstrates how digital technologies can be applied to solve real-world scientific and societal challenges.

The ACMS is therefore not intended to replace human cave researchers. Instead, it aims to make caves digitally accessible, scientifically documented, and protected for future generations.

This creates a meaningful balance between research, education, public accessibility, and environmental conservation.

3. Data and AI Techniques

The planned Autonomous Cave Mapping System (ACMS) is based on collecting and processing various data sources gathered during an autonomous exploration mission within a cave system. The quality and availability of these data are crucial to the project’s success because they form the foundation for both autonomous navigation and the later creation of a digital 3D model.

The most important data source consists of high-resolution images of cave walls, ceilings, and floor areas. These images are captured either at fixed intervals or according to the distance traveled by the drone. With sufficient overlap between images, photogrammetric techniques can later be applied to generate a detailed three-dimensional model of the cave. Additionally, video recordings can be used to document movement sequences and special events during the mission.

Beyond image data, various sensor measurements are employed. These include LiDAR or depth-sensor distance measurements, acceleration and angular velocity data from an Inertial Measurement Unit (IMU), altitude information, and potentially environmental data such as temperature and humidity. These sensor inputs support localization and the generation of a three-dimensional environmental map. Since GPS signals are unavailable inside caves, all navigation decisions must be based on locally acquired data.

Another potential data source consists of existing cave survey records. Many caves have already been documented through manual surveying. These historical datasets can serve as references and be compared with newly collected measurements, allowing assessment of mapping accuracy and identification of changes within the cave.

In the field of Artificial Intelligence, several approaches are applicable. For autonomous navigation, the drone can utilize Simultaneous Localization and Mapping (SLAM) methods. These algorithms allow the system to build a map while simultaneously determining its position within that map. AI-supported obstacle detection techniques can also be employed to recognize rock formations, narrow passages, and other hazards early enough to avoid collisions.

Furthermore, machine learning methods could be used to automatically identify interesting geological structures. For example, stalactite formations, mineral deposits, or other geological features could be detected and marked for more detailed documentation. Automated image-quality assessment could also identify blurred or poorly illuminated images during the mission.

For an initial project demonstration, a prototype can be developed that processes real image and sensor data. Test data from caves or artificially created environments may be used. Using Python and freely available libraries such as OpenCV, Open3D, COLMAP, and ROS2, initial image-processing, mapping, and navigation functions can be implemented and evaluated. This allows early validation of the selected data sources and AI techniques before developing a complete ACMS.

The combination of high-resolution image data, sensor measurements, and modern AI techniques therefore forms the foundation for autonomous cave exploration, documentation, and digital reconstruction. At the same time, it enables the enhancement of existing surveys, supports scientific investigations, and promotes long-term digital accessibility of cave systems.

4. How Will It Be Used?

The Autonomous Cave Mapping System (ACMS) is intended for the autonomous acquisition and documentation of cave systems. For this purpose, a drone equipped with cameras and sensors is launched from a defined entry point within a cave. During the mission, the system moves independently through the cave and collects image and sensor data from the surrounding environment. After completing the data acquisition process, the drone returns to its starting point and transfers the collected data for further processing.

The information gathered during the exploration is subsequently analyzed using a powerful computer system. By applying photogrammetry and 3D reconstruction techniques, a digital model of the cave is created that can be used for documentation, research, and presentation purposes. The system is not intended to replace cave researchers but rather to complement existing documentation methods and improve the digital accessibility of cave systems.

The primary application area of the project is cave research and cave documentation. In particular, members of the Kluterthöhle Working Group (AKKH) can benefit from such a system. Many members possess extensive knowledge of the cave and have contributed to its surveying and documentation over many years. The data generated by ACMS can help verify, supplement, and archive existing survey data. At the same time, a digital model provides access to areas that cannot always be explored or can only be reached with considerable effort.

Another important target group consists of club members who can no longer actively participate in cave expeditions due to age or physical limitations. Through digital reconstruction, these individuals can continue to explore the cave virtually and remain involved in research and documentation activities. The system therefore helps preserve and share knowledge and experience within the organization over the long term.

In addition, the project may also be valuable to the general public. Many people are interested in caves and geological features but do not have the opportunity to visit them personally. Reasons may include physical limitations, safety requirements, or conservation measures designed to protect sensitive cave environments. A digital 3D model provides a realistic insight into the cave without requiring additional visitors to enter the natural environment.

The system also offers advantages from a conservation perspective. The number of necessary cave visits can be reduced, thereby providing better protection for fragile geological structures. At the same time, scientific documentation and public education remain possible. The project therefore seeks to balance the interests of research, conservation, community organizations, and the public.

When considering the stakeholders affected by the project, several perspectives must be taken into account. Cave researchers require highly accurate and scientifically valuable data. Club members expect long-term preservation of documentation and improved access to research results. Conservationists advocate for the most careful treatment possible of sensitive cave systems. The public benefits from improved access to knowledge and information about geological natural monuments. ACMS aims to integrate these diverse requirements into a single technical solution.

5. Challenges

Which Problems Are Not Solved by the Project?

The Autonomous Cave Mapping System (ACMS) is intended to improve the digital documentation and virtual accessibility of cave systems. However, the system cannot solve all challenges associated with cave research and cave documentation. Like any technological solution, ACMS has technical, organizational, and scientific limitations.

First and foremost, the system does not replace experienced cave researchers. The interpretation of geological structures, the scientific evaluation of observations, and the planning of complex research projects still require human expertise. ACMS can collect and provide data, but the actual analysis and scientific interpretation remain the responsibility of specialists.

Similarly, the system cannot completely replace the direct experience of being inside a cave. Although a digital 3D model can provide a highly realistic impression, personal experiences, spatial perception, and immediate on-site observations can only be represented digitally to a limited extent. ACMS is therefore intended as a supplement rather than a complete alternative to traditional cave exploration.

Another limitation concerns the accessibility of all cave areas. Narrow crevices, flooded passages, strong air currents, or complex vertical shafts may prevent an autonomous drone from exploring certain sections or may significantly restrict its capabilities. Consequently, the system may not be able to document every cave completely.

Furthermore, the quality of the generated 3D models depends directly on the quality of the collected data. Poor lighting conditions, dust, fog, humidity, or sensor malfunctions can negatively affect measurement accuracy. Although the system may employ error-detection and quality-control mechanisms, completely error-free data collection cannot be guaranteed.

The system also cannot prevent changes within the cave itself. Natural processes such as speleothem growth, erosion, water movement, or rockfalls occur independently of any documentation efforts. ACMS can record and document such changes but cannot influence them.

Another important consideration is cave protection. While ACMS can help reduce the number of required cave visits, it cannot guarantee that no damage will occur. Operating a drone still requires people to enter the cave and therefore involves a residual risk to the sensitive environment. Appropriate conservation measures and environmental protection guidelines must therefore continue to be observed.

Finally, the project does not solve the problem of long-term digital data preservation. The generated image, sensor, and 3D data must be stored, managed, and regularly backed up. Without suitable archiving strategies, valuable information may be lost over time.

In summary, ACMS is a tool that supports research, documentation, and knowledge transfer. It can automate data collection, improve digital accessibility, and contribute to the protection of sensitive cave systems. However, scientific interpretation, practical cave exploration, and the long-term preservation of information remain human responsibilities.

An additional advantage of acknowledging these limitations is that it demonstrates to evaluators that the project is not presented as a universal solution. Instead, it shows a conscious awareness of the boundaries of artificial intelligence, robotics, and digitalization, which is often viewed positively during project evaluations.

6. What Comes Next?

Future Development of the Project

The Autonomous Cave Mapping System (ACMS) is designed as an initial functional approach to autonomous data acquisition in caves. However, it has significant potential for long-term development and expansion. The current focus is on collecting image and sensor data and generating a 3D model on an external computer system. Building on this foundation, several future development stages can be envisioned.

A natural next step is improving the autonomy of the drone. Future versions could not only collect data but also make more complex decisions independently, such as determining optimal exploration routes, prioritizing unknown areas, or dynamically adapting to challenging environmental conditions. This would transform the system from a simple data-collection platform into an intelligent exploration system.

Another important area of development concerns sensor technology. In addition to cameras and basic navigation sensors, future versions could integrate high-resolution LiDAR systems, multispectral cameras, or thermal sensors. This would significantly improve the quality of 3D reconstruction while also enabling additional scientific insights into the cave environment.

In the long term, multi-drone systems could also be considered. Several autonomous units could simultaneously explore different areas of a cave, communicate with one another, and coordinate their data collection. This would allow larger cave systems to be documented more efficiently and comprehensively. Related developments could include radio or optical relay systems to ensure communication in deep or highly branched cave networks.

Another development path involves real-time 3D modeling. Instead of processing data only after the mission, future versions of the system could continuously generate and update a 3D model during flight. This capability would not only improve navigation but also enable faster analysis and decision-making.

Furthermore, ACMS could be expanded with advanced artificial intelligence capabilities beyond navigation. Examples include automatic classification of geological structures, detection of changes compared with historical datasets, and identification of particularly sensitive or protected areas within a cave.

The practical application of the system beyond cave exploration also represents a promising development opportunity. The technology could potentially be used in underground mines, tunnel systems, disaster zones, or difficult-to-access infrastructure facilities. This would significantly broaden its range of applications and make it attractive for industrial and safety-related scenarios.

Overall, ACMS offers considerable development potential. It can evolve from a basic autonomous exploration platform into a highly integrated system for autonomous exploration, 3D digitization, and intelligent environmental analysis. In the long term, this could make the system valuable not only for cave research but also for numerous fields of robotics and environmental monitoring.

7. Acknowledgements

The Autonomous Cave Mapping System (ACMS) project is currently in an early conceptual phase. At the present time, no concrete software implementation has been developed, and no open-source software components have been incorporated. Therefore, there are currently no direct software or code sources that need to be cited within the scope of the project.

The fundamental idea and motivation behind the project are strongly influenced by practical activities in the field of cave exploration. In particular, the Kluterthöhle Working Group (AKKH) has served as a major source of inspiration. Through membership in the organization and interaction with fellow cave researchers, valuable insights were gained into the challenges of surveying, documenting, and exploring cave systems.

Experiences gained through practical work within the AKKH have played a significant role in defining the project’s objectives. In particular, they highlighted how time-consuming manual surveying can be and how important it is to achieve detailed documentation while minimizing impact on sensitive cave environments.

Additional inspiration comes from current research in autonomous robotics and cave exploration, particularly international projects focusing on autonomous navigation and 3D mapping in GPS-denied environments. These research efforts serve as conceptual guidance for the future development of ACMS, although no specific implementations have been adopted at the current stage of the project.

In summary, the project is currently based primarily on original conceptual work, complemented by practical experience gained through activities within the AKKH and by scientific inspiration from contemporary research in autonomous systems and cave exploration.



