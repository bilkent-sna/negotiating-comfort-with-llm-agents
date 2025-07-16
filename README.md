# Code for the paper: Negotiating Comfort: Simulating Personality-Driven LLM Agents in Shared Residential Social Networks

In this repository, we provide the code for the simulation and analysis stages of the study, as well as the important result files used in the analysis.

- Initial graph can be found on: [families3.json](energy_sim_1\families3.json)
- List of families can be found on: [family_members3.json](energy_sim_1\family_members3.json)
- Graph data saved by Crowd in each snapshot period and the LLM query outputs are not uploaded to the repository due to their large file sizes. Other data files can be found on: [energy_sim_1\results](energy_sim_1\results)

# Steps to set up

In this study, we utilize our social network simulation library, [Crowd](https://crowd.readthedocs.io/en/latest/) and run our simulations on Google Colab with an L4 GPU.

To use Crowd in Google Colab, first download the wheel file:

1. Go to [Crowd's repository](https://github.com/bilkent-sna/crowd)
2. Navigate to releases page of the repository and download the latest .whl file

Upload the wheel file and _negotiating_comfort.ipynb_ to Google Drive and follow the steps provided in the notebook.

# Additional code files

- _analysis.ipynb_: Node-level statistical analysis with Fixed Effects and Correlated Random Effects models (Panel Data Analysis)
- _analysis_network_level.ipynb_: Network-level statistical analysis with Ordinary Least Squares (OLS) regression

## Citation

If you find this repository helpful, please cite the following paper:
`    @misc{rende2025negotiatingcomfortsimulatingpersonalitydriven,
        title={Negotiating Comfort: Simulating Personality-Driven LLM Agents in Shared Residential Social Networks}, 
        author={Ann Nedime Nese Rende and Tolga Yilmaz and Özgür Ulusoy},
        year={2025},
        eprint={2507.09657},
        archivePrefix={arXiv},
        primaryClass={cs.SI},
        url={https://arxiv.org/abs/2507.09657}, 
    }
   `

Additionally, consider citing the following paper if you use Crowd:

```
@article{rende2025crowd,
   title={Crowd: A Social Network Simulation Framework},
   author={Rende, Ann Nedime Nese and Yilmaz, Tolga and Ulusoy, Ozgur},
   journal={IEEE Transactions on Computational Social Systems},
   year={2025},
   publisher={IEEE},
   doi={10.1109/TCSS.2025.3565377}
}
```
