# master-large-scale-algorithms
Master Building Large Scale Algorithms

## ✅ Setup Env
- Create Python environment\
`conda create -n env_name python=3.10`\
`conda activate env_name`
- Create Python environment\
`pip install -r .\path_to_requirements\requirements.txt`

## ✅ Large-scale algorithms
- A well-designed, large-scale algorithm:
  - Characteristics:
    - It is designed to handle a huge amount of data and processing requirements using an available pool of resources optimally.
    - It is scalable. As the problem becomes more complex, it can handle the complexity simply by provisioning more resources.
  - One of the most practical way of implementing large-scale algorithms is by using the divide and conquer strategy,that is, divide the larger problem into smaller problems that can be solved independently of each other.  
  - Terminology
    - Latency: end-to-end time taken to perform a single computation
    - Throughput: In the context of parallel computing, throughput is the number of single computations that can be performed simultaneously.
    - Network bisection bandwidth: The bandwidth between two equal parts of a network is called the network bisection bandwidth. For distributed computing to work efficiently, this is the most important parameter to consider. If we do not have enough network bisection bandwidth, the benefits gained by the availability of multiple execution engines in distributed computing will be overshadowed by slow communication links.
    - Elasticity: The ability of the infrastructure to react to a sudden increase in processing requirements by provisioning more resources is called elasticity. 
- Parallel algorithm
  - Amdahl's law: It is based on the concept that in any computing process, not all of the processes can be executed in parallel. There will be a sequential portion of the process that cannot be parallelized.
  - we need to find more than one execution engines running in parallel to solve a complex problem:
    - Look within: Exploit the resources already on the computer. Use the hundreds of cores of the GPU to run a large-scale algorithm.
    - Look outside: Use distributed computing to find more computing resources that can be collectively used to solve the large-scale problem at hand.
    - Hybrid strategy: Use distributed computing and, on each of the nodes, use the GPU or an array of GPUs to expedite the running of the algorithm.
- Algorithms to utilize the GPU
  - Mining money for bitcoins 
  - Large-scale simulations 
  - DNA analysis 
  - Video and photos analysis
- Algorithms utilizing cluster computing
  - Multiple nodes connected via a very high-speed network. 
  - Large-scale algorithms are submitted as jobs. 
  - Each job is divided into various tasks and each task is run on a separate node.
  - Apache Spark: Resilient Distributed Datasets (RDDs)
- Using GPU to run large-scale algorithms
- Using clusters to run large-scale algorithms