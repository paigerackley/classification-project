# <a name="top"></a>README TITLE
2
![]()
3

4
by: Paige Rackley
5

6
<p>
7
  <a href="https://github.com/mdalton87" target="_blank">
8
    <img alt="Matthew" src="https://img.shields.io/github/followers/mdalton87?label=Follow_Matt&style=social" />
9
  </a>
10
</p>
11

12

13
***
14
[[Project Description](#project_description)]
15
[[Project Planning](#planning)]
16
[[Key Findings](#findings)]
17
[[Data Dictionary](#dictionary)]
18
[[Data Acquire and Prep](#wrangle)]
19
[[Data Exploration](#explore)]
20
[[Statistical Analysis](#stats)]
21
[[Modeling](#model)]
22
[[Conclusion](#conclusion)]
23
___
24

@mdalton87
update
13 months ago
25
<img src="https://docs.google.com/drawings/d/e/2PACX-1vR19fsVfxHvzjrp0kSMlzHlmyU0oeTTAcnTUT9dNe4wAEXv_2WJNViUa9qzjkvcpvkFeUCyatccINde/pub?w=1389&amp;h=410">
@mdalton87
added images
13 months ago
26

27
## <a name="project_description"></a>Project Description:
28
[[Back to top](#top)]
29

30
***
31
## <a name="planning"></a>Project Planning: 
32
[[Back to top](#top)]
33

34
### Project Outline:
35

36

37

38
### Hypothesis
39

40

41

42
### Target variable
43

44

45
### Need to haves (Deliverables):
46

47

48

49
### Nice to haves (With more time):
50

51

52

53
***
54

55
## <a name="findings"></a>Key Findings:
56
[[Back to top](#top)]
57

58

59

60

61
***
62

63
## <a name="dictionary"></a>Data Dictionary  
64
[[Back to top](#top)]
65

66
### Data Used
67
---
68
| Attribute | Definition | Data Type |
69
| ----- | ----- | ----- |
70
| | | |
71
| | | |
72
| | | |
73
| | | |
74
| | | |
75
| | | |
76

77
***
78

79
## <a name="wrangle"></a>Data Acquisition and Preparation
80
[[Back to top](#top)]
81

82
![]()
83

84

85
### Wrangle steps: 
86

87

88
*********************
89

90
## <a name="explore"></a>Data Exploration:
91
[[Back to top](#top)]
92
- Python files used for exploration:
93
    - wrangle.py 
94
    - explore.py
95
    - modeling.py
96

97

98
### Takeaways from exploration:
99

100

101
***
102

103
## <a name="stats"></a>Statistical Analysis
104
[[Back to top](#top)]
105

106
### Stats Test 1: ANOVA Test: One Way
107

108
Analysis of variance, or ANOVA, is a statistical method that separates observed variance data into different components to use for additional tests. 
109

110
A one-way ANOVA is used for three or more groups of data, to gain information about the relationship between the dependent and independent variables: in this case our clusters vs. the log_error, respectively.
111

112
To run the ANOVA test in Python use the following import: \
113
<span style="color:green">from</span> scipy.stats <span style="color:green">import</span> f_oneway
114

115
- f_oneway, in this case, takes in the individual clusters and returns the f-statistic, f, and the p_value, p:
116
    - the f-statistic is simply a ratio of two variances. 
117
    - The p_vlaue is the probability of obtaining test results at least as extreme as the results actually observed, under the assumption that the null hypothesis is correct
118

119
#### Hypothesis:
120
- The null hypothesis (H<sub>0</sub>) is
121
- The alternate hypothesis (H<sub>1</sub>) is 
122

123
#### Confidence level and alpha value:
124
- I established a 95% confidence level
125
- alpha = 1 - confidence, therefore alpha is 0.05
126

127
#### Results:
128

129

130
#### Summary:
131

132

133
### Stats Test 2: T-Test: One Sample, Two Tailed
134
- A T-test allows me to compare a categorical and a continuous variable by comparing the mean of the continuous variable by subgroups based on the categorical variable
135
- The t-test returns the t-statistic and the p-value:
136
    - t-statistic: 
137
        - Is the ratio of the departure of the estimated value of a parameter from its hypothesized value to its standard error. It is used in hypothesis testing via Student's t-test. 
138
        - It is used in a t-test to determine if you should support or reject the null hypothesis
139
        - t-statistic of 0 = H<sub>0</sub>
140
    -  - the p-value:
141
        - The probability of obtaining test results at least as extreme as the results actually observed, under the assumption that the null hypothesis is correct
142
- We wanted to compare the individual clusters to the total population. 
143
    - Cluster1 to the mean of ALL clusters
144
    - Cluster2 to the mean of ALL clusters, etc.
145

146
#### Hypothesis:
147
- The null hypothesis (H<sub>0</sub>) is 
148
- The alternate hypothesis (H<sub>1</sub>) is 
149

150
#### Confidence level and alpha value:
151
- I established a 95% confidence level
152
- alpha = 1 - confidence, therefore alpha is 0.05
153

154

155
#### Results:
156

157

158
#### Summary:
159

160
***
161

162
## <a name="model"></a>Modeling:
163
[[Back to top](#top)]
164

165
### Model Preparation:
166

167
### Baseline
168

169
- Baseline Results: 
170

171

172
- Selected features to input into models:
173
    - features = []
174

175
***
176

177
### Models and R<sup>2</sup> Values:
178
- Will run the following regression models:
@mdalton87
update
13 months ago
179

@mdalton87
added images
13 months ago
180

181

182
- Other indicators of model performance with breif defiition and why it's important:
@mdalton87
update
13 months ago
183

@mdalton87
added images
13 months ago
184

185

186
#### Model 1: Linear Regression (OLS)
187

188

189
- Model 1 results:
190

191

192

193
### Model 2 : Lasso Lars Model
194

195

196
- Model 2 results:
197

198

199
### Model 3 : Tweedie Regressor (GLM)
200

201
- Model 3 results:
202

203

204
### Model 4: Quadratic Regression Model
205

206
- Model 4 results:
207

208

209
## Selecting the Best Model:
210

211
### Use Table below as a template for all Modeling results for easy comparison:
212

213
| Model | Validation/Out of Sample RMSE | R<sup>2</sup> Value |
214
| ---- | ----| ---- |
215
| Baseline | 0.167366 | 2.2204 x 10<sup>-16</sup> |
216
| Linear Regression (OLS) | 0.166731 | 2.1433 x 10<sup>-3</sup> |  
217
| Tweedie Regressor (GLM) | 0.155186 | 9.4673 x 10<sup>-4</sup>|  
218
| Lasso Lars | 0.166731 | 2.2204 x 10<sup>-16</sup> |  
219
| Quadratic Regression | 0.027786 | 2.4659 x 10<sup>-3</sup> |  
220

221

222
- {} model performed the best
223

224

225
## Testing the Model
226

227
- Model Testing Results
228

229
***
230

231
## <a name="conclusion"></a>Conclusion:
232
[[Back to top](#top)]
