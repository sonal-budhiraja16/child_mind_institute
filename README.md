# child_mind_institute

**Overview**

The repository is being setup to solve the follwong problem hosted by Kaggle. Details are available on this link- https://www.kaggle.com/competitions/child-mind-institute-problematic-internet-use

Description
In today’s digital age, problematic internet use among children and adolescents is a growing concern. Better understanding this issue is crucial for addressing mental health problems such as depression and anxiety.

Current methods for measuring problematic internet use in children and adolescents are often complex and require professional assessments. This creates access, cultural, and linguistic barriers for many families. Due to these limitations, problematic internet use is often not measured directly, but is instead associated with issues such as depression and anxiety in youth.

Conversely, physical & fitness measures are extremely accessible and widely available with minimal intervention or clinical expertise. Changes in physical habits, such as poorer posture, irregular diet, and reduced physical activity, are common in excessive technology users. We propose using these easily obtainable physical fitness indicators as proxies for identifying problematic internet use, especially in contexts lacking clinical expertise or suitable assessment tools.

This competition challenges you to develop a predictive model capable of analyzing children's physical activity data to detect early indicators of problematic internet and technology use. This will enable prompt interventions aimed at promoting healthier digital habits.


**Evaluation**
Submissions are scored based on the quadratic weighted kappa, which measures the agreement between two outcomes. This metric typically varies from 0 (random agreement) to 1 (complete agreement). In the event that there is less agreement than expected by chance, the metric may go below 0.

To compute the quadratic weighted kappa, we construct three matrices, O, W, and E, with N the number of distinct labels.

The matrix \$O\$ is an \$NxN\$ histogram matrix such that \$O_{i,j}\$   corresponds to the number of instances that have an actual value \$i\$ and a predicted value \$j\$.

The matrix \$W\$ is an \$NxN\$ matrix of weights, calculated based on the squared difference between actual and predicted values: \$\W_{i,j} = (i−j)^2(N−1)^2\$

The matrix \$E$ is an \$NxN\$ histogram matrix of expected outcomes, calculated assuming that there is no correlation between values. This is calculated as the outer product between the actual histogram vector of outcomes and the predicted histogram vector, normalized such that \$E$ and \$O$ have the same sum.

From these three matrices, the quadratic weighted kappa is calculated as: 

\$κ=1−∑_{i,j} W_{i,j} O_{i,j} ∑_{i,j} W_{i,j}E_{i,j}\$.
Your work will contribute to a healthier, happier future where children are better equipped to navigate the digital landscape responsibly.
