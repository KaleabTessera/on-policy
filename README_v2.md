# Steps to Run 8m
1. Create conda env using environment file:
    ```
    conda env create --name marl --file=environment.yaml
    ```

2. Activate env:
    ```
    conda activate marl
    ```

3. Install pytorch:
    ```
    pip install torch==1.5.1+cu101 torchvision==0.6.1+cu101 -f https://download.pytorch.org/whl/torch_stable.html
    ```

4. Install onpolicy repo:
    ```
    pip install -e .
    ```

5. Run 8m:
    ```
    # Install Smac - https://github.com/marlbenchmark/on-policy#21-starcraftii-410
    # Set SMAC location 
    export SC2PATH=[]
    # Run 8m 
    cd ./onpolicy/scripts/train_smac_scripts && ./train_smac_8m.sh
    ```


