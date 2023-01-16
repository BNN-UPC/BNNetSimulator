# BNNetSimulator

BNNetSimulator is a packet-level network simulator that is built on the OMNeT++ framework. It allows users to easily generate network datasets for research and analysis. With BNNetSimulator, you can define a network topology with various node and link features, specify a src-dst routing, and set a traffic matrix. The simulator then provides performance metrics such as mean delay, jitter, and packet loss per path, as well as link utilization and QoS queue statistics. With the [datanetAPI](https://github.com/BNN-UPC/datanetAPI/tree/BNNetSimulator) tool, you can easily process and analyze the generated dataset.

  

## Parameters

BNNetSimulator offers a variety of parameters that allow you to customize the simulation to your specific needs. You can define several characteristics for each node in the topology, including:

- The scheduling policy used to serve packets and the buffer size of the queues

- The capacities of the links

- The src-dst routing

The simulator also supports different types of traffic profiles, including:

- Poisson distribution

- CBR (Constant Bit Rate) distribution

- ON-OFF distribution

Additionally, you can define the packet size distribution as a list of packet sizes and their probabilities. For more information on the available parameters and how to use them, please refer to the [input_parameters_glossary.ipynb](input_parameters_glossary.ipynb) document.

  
  

The BNNetSimulator is available as a pre-built docker image, which can be found at https://hub.docker.com/r/bnnupc/bnnetsimulator. To use it, you can simply follow the code examples provided in the Jupyter Notebooks of the accompanying repository.

The repository includes two main Jupyter Notebooks that will guide you through the process of using the simulator:

- [quickstart.ipynb](quickstart.ipynb): This notebook provides a step-by-step introduction to the process of generating your first dataset using the BNNetSimulator. It covers all the necessary steps and provides clear examples to help you get started.

- [input_parameters_glossary.ipynb](input_parameters_glossary.ipynb): This notebook contains detailed descriptions of the various parameters that can be used to build a dataset. It provides information on what each parameter does, how to use it, and how it affects the resulting dataset.

  

Both the quickstart.ipynb and input_parameters_glossary.ipynb are a great resources for someone who wants to get started using BNNetSimulator.

  

## Cite the simulator

Please, if you use the simulator, don't forget to use the following citation:

**<u>Plain text:</u>**

Miquel Ferriol-Galmés, Jordi Paillisse, José Suárez-Varela, Krzysztof Rusek, Shihan Xiao, Xiang Shi, Xiangle Cheng, Pere Barlet-Ros, and Albert Cabellos-Aparicio. (2022). RouteNet-Fermi: Network Modeling with Graph Neural Networks. arXiv preprint arXiv:2212.12070.

**<u>BibTeX:</u>**

```

@article{ferriol2022routenet,

title={RouteNet-Fermi: Network Modeling with Graph Neural Networks},

author={Ferriol-Galm{\'e}s, Miquel and Paillisse, Jordi and Su{\'a}rez-Varela, Jos{\'e} and Rusek, Krzysztof and Xiao, Shihan and Shi, Xiang and Cheng, Xiangle and Barlet-Ros, Pere and Cabellos-Aparicio, Albert},

journal={arXiv preprint arXiv:2212.12070},

year={2022}

}

```

  

## Setting up the docker enviroment

  

To use the BNNetSimulator, you will need to have either Docker Engine or Docker Desktop installed on your machine. Both of these tools provide a way to run the BNNetSimulator as a Docker container, which makes it easy to set up and use.

  

Here are the links to the instructions for installing Docker on your machine, depending on your operating system:

  

- Docker Desktop: https://docs.docker.com/desktop/

- Docker Engine: https://docs.docker.com/engine/

  

Make sure to follow the instructions for your specific operating system, and have the software installed before you try to use the BNNetSimulator. And in case you are having some troubles, you can always refer to the official documentation.