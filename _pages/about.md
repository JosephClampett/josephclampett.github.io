---
permalink: /
author_profile: true
redirect_from: 
  - /about/
  - /about.html

lab_gallery:
  title: "LAB"
  images:
    - image_path: "MainGallery/Lab/PXL_20240820_195800127.jpg"
    - image_path: "MainGallery/Lab/DSC_1210.jpg"
      alt: "UNC Science Expo"
    - image_path: "MainGallery/Lab/DSC_1548.jpg"
      alt: "Electromagnetic shaker with pneumatic air bearing and control system, droplet generator, compressed air for experiment pressurization, and high-speed camera"
      
nature_gallery:
  title: "SUSTAINABILITY"
  images:
    - image_path: "MainGallery/Sustainability/DSC_0981.jpg"
      alt: "FREIBURG, Germany - Inside wind turbine purchased by farmer collective"
    - image_path: "MainGallery/Sustainability/DSC_0031.jpg"
      alt: "FREIBURG, Germany - Green roofs at Solar Info Center"
    - image_path: "MainGallery/Sustainability/DSC_1267.jpg"
      alt: "BASEL, Switzerland - Green buildings in Basel shopping center"
    - image_path: "MainGallery/Sustainability/DSC_1415.jpg"
      alt: "VAUBAN, Germany - Custom development of net-zero buildings"
    - image_path: "MainGallery/Sustainability/DSC_1824.jpg"
      alt: "ROTTERDAM, Netherlands - GE Haliade X 14 offshore wind turbine - test unit installed onshore"
    - image_path: "MainGallery/Sustainability/DSC_1862.jpg"
      alt: "ROTTERDAM, Netherlands - Transition pieces awaiting installation at Port of Rotterdam"
    - image_path: "MainGallery/Sustainability/DSC_3566.jpg"
      alt: "CROYDON, England - Tramlink service center in London"
    - image_path: "MainGallery/Sustainability/DSC_3673.jpg"
      alt: "HULL, England - University of Hull Innovation Center x Siemens Gamesa project to optimize turbine coatings"
    - image_path: "MainGallery/Sustainability/DSC_0771.jpg"
      alt: "VAUBAN, Germany - Residents collaborated with architects to design custom net-zero housing projects"
    - image_path: "MainGallery/Sustainability/DSC_3798.jpg"
      alt: "HULL, England - Inside Ørsted control center for largest wind turbine farms in the world" 
    - image_path: "MainGallery/Sustainability/DSC_4973.jpg"
      alt: "Washington, USA - Solar panels on federal buildings - General Services Administration has millions for building energy efficiency upgrades"
    - image_path: "MainGallery/Sustainability/DSC_9949.jpg"
      alt: "FREIBURG, England - Redesigned streets for trams, cars, hiking, and pedestrians" 
    - image_path: "MainGallery/Sustainability/PXL_20241005_060357726.jpg"
      alt: "台北, 台灣 (TAIPEI, Taiwan) - Reloctable LFP battery system at Energy Taiwan 2024 conference" 
    - image_path: "MainGallery/Sustainability/DSC_2394.jpg"
      alt: "LONDON, ENGLAND - Ed Miliband, now-UK Secretary of State for Energy Security and Net Zero, delivers Labour's vision for clean energy at the Global Offshore Wind Conference 2023" 
    - image_path: "MainGallery/Sustainability/DSC_1703.jpg"
      alt: "ROTTERDAM, Netherlands - Company building products out of algae at cleantech innovation hub in Rotterdam" 
    - image_path: "MainGallery/Sustainability/DSC_1827.jpg"
      alt: "ROTTERDAM, Netherlands - Experimental floating offshore wind farm at Port of Rotterdam" 
      
photography_gallery:
  title: "PHOTOGRAPHY"
  images:
    - image_path: "MainGallery/Photography/Clampett_London_England.png"
      alt: "LONDON, England" 
    - image_path: "MainGallery/Photography/DSC_7953.jpg"
      alt: "台北, 台灣 (TAIPEI, Taiwan)" 
    - image_path: "MainGallery/Photography/Clampett_Zürich_Switzerland.png"
      alt: "ZÜRICH, Switzerland" 
    - image_path: "MainGallery/Photography/DSC_0297.jpg"
      alt: "RIBEAUVILLÉ, France (Roof of Catholic  church)" 
    - image_path: "MainGallery/Photography/DSC_1544-2.jpg"
      alt: "SANTA MONICA, California" 
    - image_path: "MainGallery/Photography/DSC_4251.jpg"
      alt: "LONDON, England" 
    - image_path: "MainGallery/Photography/DSC_6459.jpg"
      alt: "Greensboro, North Carolina - My backyard" 
    - image_path: "MainGallery/Photography/DSC_7108.jpg"
      alt: "MT PILATUS, Switzerland" 
    - image_path: "MainGallery/Photography/DSC_7958.jpg"
      alt: "象山, 台灣 (XIANGSHAN, Taiwan)" 
    - image_path: "MainGallery/Photography/DSC_8014.jpg"
      alt: "象山, 台灣 (XIANGSHAN, Taiwan)" 
    - image_path: "MainGallery/Photography/DSC_8173.jpg"
      alt: "COUNTY WICKLOW, Ireland"
    - image_path: "MainGallery/Photography/DSC_8524.jpg"
      alt: "中山, 台灣 (ZHONGSHAN, Taiwan)" 
    - image_path: "MainGallery/Photography/DSC_9572.jpg"
      alt: "台大, 台灣 (NTU, Taiwan)" 
    - image_path: "MainGallery/Photography/DSC_1759.jpg"
      alt: "SAN FRANSISCO, California" 
      
visualization_gallery:
  title: "VISUALIZATIONS"
  images:
    - image_path: "MainGallery/Visualization/DSC_0028.jpg"
    - image_path: "MainGallery/Visualization/DSC_0035.jpg"
---

{% include gallery id="lab_gallery" %}
{% include gallery id="nature_gallery" %}
{% include gallery id="photography_gallery" %}

{% include gallery id="visualization_gallery" %}
<figure class="half">
  <figure width="50%">
    <video autoplay muted loop width="100%">
      <source src="{{base_path}}/images/MainGallery/Visualization/04_2024-08-16-184411-0000.mp4" type="video/mp4">
    </video>
    <figcaption>Faraday Waves visualized with semireflective mirror</figcaption>
  </figure>
  <figure width="50%">
    <video autoplay muted loop width="100%">
    <source src="{{base_path}}/images/MainGallery/Visualization/Game.mp4" type="video/mp4">
    </video>
  <figcaption>Two-player realtime interactive game made in a week for visualization competition</figcaption>
  </figure>
</figure>
