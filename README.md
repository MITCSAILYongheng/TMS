# TransMetaSegmentation (TMS) extends mass spectrometry imaging to single-cell resolution

This document describes the 4 steps required to co-register images from mass spectrometry imaging (MSI) and single-cell spatial transcriptomics (SST), segment the MSI image using the cell boundary and cell type information from the SST image, and quantify the metabolite signal in individual cells.

### Step 1: Export the csv file from the SCiLS Lab software

![Export](https://github.com/user-attachments/assets/4fff0a62-1ad3-4273-b1ce-cafbff043b35)

### Step 2: Convert csv file to an MSI image

https://github.com/user-attachments/assets/32300baf-3b86-4267-8918-cde93aa0fe22

A high-resolution video is available here: https://www.youtube.com/watch?v=s7_lwnretkI

The values in the following 4 locations needed to be changed based on the metabolite and CSV file size.

1. target_value = 885.5360
  
2. tolerance = 0.0088 
 
3. Numbers within range 885.5272 to 885.5447999999999 are found at positions: [77854, 77855, 77856]

4. end_row = 281  

Please note the largest Sum value printed. We will use this value in step 4. In this example, it is: "Spot Spot 206569: Sum = 1663.5873994143".

### Step 3: Extract the cell boundary and cell type information from SST image

https://github.com/user-attachments/assets/ae9332b0-86fe-4cd5-b855-65d9058e8554

A high-resolution video is available here: https://www.youtube.com/watch?v=N6qMOrSuZVA

### Step 4: Co-register MSI and SST images to measure metabolite signal in each cell

https://github.com/user-attachments/assets/9bc89542-3d38-437c-a069-a04b5b0dea8d

A high-resolution video is available here: https://www.youtube.com/watch?v=DPfilnj4YTk

Replace the value max_spot_sum = 266.74240094392 with the maximum Sum value from step 2: 1663.5873994143.

