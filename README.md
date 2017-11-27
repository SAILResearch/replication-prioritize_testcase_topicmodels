# Replication Package for "Static Test Case Prioritization Using Topic Models"

Stephen W. Thomas, Hadi Hemmati, Ahmed E. Hassan, and Dorothea Blostein  
[Empirical Software Engineering journal, vol. 19, issue 1, 2014](http://dx.doi.org/10.1007/s10664-012-9219-7)

Abstract: Software development teams use test suites to test changes to their source code. In many situations, the test suites are so large that executing every test for every source code change is infeasible, due to time and resource constraints. Development teams need to prioritize their test suite so that as many distinct faults as possible are detected early in the execution of the test suite. We consider the problem of static black-box test case prioritization (TCP), where test suites are prioritized without the availability of the source code of the system under test (SUT). We propose a new static black-box TCP technique that represents test cases using a previously unused data source in the test suite: the linguistic data of the test cases, i.e., their identifier names, comments, and string literals. Our technique applies a text analysis algorithm called topic modeling to the linguistic data to approximate the functionality of each test case, allowing our technique to give high priority to test cases that test different functionalities of the SUT. We compare our proposed technique with existing static black-box TCP techniques in a case study of multiple real-world open source systems: several versions of Apache Ant and Apache Derby. We find that our static black-box TCP technique outperforms existing static black-box TCP techniques, and has comparable or better performance than two existing execution-based TCP techniques. Static black-box TCP methods are widely applicable because the only input they require is the source code of the test cases themselves. This contrasts with other TCP techniques which require access to the SUT runtime behavior, to the SUT specification models, or to the SUT source code.

## Bibtex

If you found this replication package helpful or used it for your own project, please consider citing our original paper:

```bibtex
@Article{Thomas2014,
author="Thomas, Stephen W.
and Hemmati, Hadi
and Hassan, Ahmed E.
and Blostein, Dorothea",
title="Static test case prioritization using topic models",
journal="Empirical Software Engineering",
year="2014",
month="Feb",
day="01",
volume="19",
number="1",
pages="182--212",
issn="1573-7616",
doi="10.1007/s10664-012-9219-7",
url="https://doi.org/10.1007/s10664-012-9219-7"
}
```

## Data and Scripts

We supply the data and results for the following systems: 

- Ant v7
- Derby v1
- Derby v2
- Derby v3
- Derby v5

[Full data and results](https://github.com/SAILResearch/replication-prioritize_testcase_topicmodels/releases/latest) (3.4MB). We include a README.txt file to describe the organization of the data. 

## Tools

The ```tcp.lda``` tool can be found on [GitHub](https://github.com/stepthom/tcp.lda). 

The preprocessing tool (```lscp```) can also be found on [GitHub](https://github.com/doofuslarge/lscp). 
