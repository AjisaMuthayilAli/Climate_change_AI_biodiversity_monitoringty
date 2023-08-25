### Climate_change_AI_biodiversity_monitoring
Climate change is one of the main reasons for drastic environmental changes such as drought, flood, wild fires, excessive heat, salt water intrusion in fresh water sources due to sea level rise etc. Therefore, climate change does impact negatively on the biodiversity of the ecosystem. It results in biodiversity reduction and migration. Coral reef bleaching due to rise in ocean water temperature, reduction/migration of polar bear in arctic and extinction of bramble cay melomys are examples of climate change adverse effects. It is possible that by preserving and re-storing biodiversity, climate change can be mitigated. Machine learning (ML) can be used to identify and classify images. In this project the main objective is that researchers and conservation biologists need the daily information about number of animals sighted at various locations throughout Karoo National Park to monitor trends in biodiversity and animal populations to inform policy makers inorder to formualate policies to protect and preserve park ecosystem.

Lab1: [Snapshot Karoo dataset](https://lila.science/datasets/snapshot-karoo) were used in this lab and are already annotated via [zooinverse voluntary programme](https://www.zooniverse.org/projects/shuebner729/snapshot-karoo/classify). Explorataory data analysis and visualisation was done.

Lab2: In this lab the [MegaDetector model](https://github.com/microsoft/CameraTraps/blob/main/megadetector.md) was used to automatically identify which images in the dataset contain animals and where in each image the animal can be found. From the images captured by the pre-trained model of megadetector, the images were cropped to the size accepted by the model I will be using (square images of 244x244 pixel). 

Lab3: In this lab, developed a model for animal classification in the Karoo national park. More specifically, fine tuned a Neural Architecture Search Network ([NASNet model](https://arxiv.org/abs/1707.07012)) that was pre-trained on the [ImageNet dataset](https://www.image-net.org/index.php). First tried the NASNet model on the dataset but it did not predict the correct animal. Therefore, augmented the data (rotated/zoomed/flipped/contrasted etc.) to train the model to identify accurately, increased number of images of animal categories which had significantly less number. Created a new model by modifying NASNet model, further fine tuned the data, evaluated and visualised. 
