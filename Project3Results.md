Purpose

The purpose of the experiment is to experimentally determine if it is faster for a user to convert units using the Smart Units extension against their preferred tool.

Procedure

All tests were conducted over zoom and each tester was asked to share their screen for observations. First each tester was given a token randomly to maintain anonymity of tester data. Testers were then instructed to install the Smart Units Chrome Extension according to the instructions provided on the git hub. After the tester had the extension installed they were given a google form with 23 unit conversions and asked to complete it using both their preferred tool and the Smart Units extension. The last digit of the testers token would determine which test they would do first. If the tester had a token ending in 0,1 or 9 they would use their preferred tool first, otherwise they would use the Smart Units extentinstion first.  With our distribution of tokens this gives us an even split of which tool is going first. When taking the test we would record the amount of time it takes testers to complete the test. Testers would then repeat the same test with the order of questions shuffled using the other tool. The time it took testers to complete the test the second time was recorded. The testes were scored for accuracy taking account for factors such as changing conversion factors(as in with currency) and human rounding. 

Materials

The google form test: https://docs.google.com/forms/d/18iF8MVOL7DDZxdMJ-Ux7btvwbwoI7kG7u-jSc3kfr-E/edit

The installation instructions: https://github.com/se20z09/units_converter_extension#installation

Observations

Many participants were impressed with the Smart Units tool. They found it easy to install and found it fast and convenient to complete conversions. Besides the smart unit tool people used websites, primarily google.com and unitconverter.net to complete the conversions. People also used the built in calculator apps on their Mac and PC’s. The extension was discovered to have some issues especially around different spelling of units. If a unit was spelled or abbreviated differently than the Smart unit tool recognized it would fail to perform a calculation. Testers also denoted the issue with the lack of ability to copy and paste from the extension. After performing a conversion testers would often forget the value and have to reconvert or enter an incorrect conversion.



Time taken to Complete Conversion Test By Method
Token | Smart Units Time (S) |Non Smart Units Time (S)
------------------------------------------------------
a856375 | 227 | 557
------------------------------------------------------
a183245
273
491
a356431
200
458
a107219
190
248
a154905
226
203  #
a767026
212
140  #
a914249
228
330
a574012
598  $
286
a460979
235
--
a414030
264
--

*-- denotes refusal to Participate
** # denotes refusal to Finish
***$ denotes difficulty using tool


Analysis

While accuracy was not a primary focus of this test it was considered to ensure any differences noticed in time were not correlated to a loss or gain in accuracy. Both groups showed comparable accuracy metrics in a test of 23 unit conversions. Tests performed using smart units had an average score of 20.4/23 with a standard deviation of 1.3 points. The median score for this group was 20/23 points. On the other hand the control group had an average score of 20.4/23 with a standard deviation of 1.5 points. The median for the control group was 21/23 points. If we assume a null hypothesis that the method used to convert units dose not have an effect on the accuracy, A two sided T confidence interval test confirms the null hypothesis with a P value of 98.25%. The close distributions of accuracy on the test show that accuracy of the conversion was not impacted by the choice of conversion method.

Using the Smart Units extension the mean time to complete the test was 265.3s with a standard deviation of 119.6s. The median time was 227.5s. Without the Smart Units extension the mean time was 339.1s with a standard deviation of 148.4s. The median without Smart Units was 308s. 

These numbers were skewed by a few outlier cases. The first outlier was participant a574012  who could not figure out how to get the smart unit extension to work properly. This severely impacted the time it took the participant to complete the test. The subject figured out how to use the extension shortly into the test and after that performed comparable to other subjects. Due to their technological blunder this data point is an outlier and was discarded from further evaluation. Other participants issued their right to refuse and did not wish to complete the manual conversions resulting in them submitting their test early or refusing to take the manual conversion test all together. Participants who did not complete the test or did not take it did not have their data factored into comparative metrics. 

With the data adjusted for outliers the new overview of data statistics is as follows. For the smart units extension the mean time for completion was 228.3s with a standard deviation of 27.0s and a median of 227s. The control group had a mean of 395s with a standard deviation of 124.2s and a median of 394s.

Performing a Paired Confidence interval T test produces a P value of 0.908% and a non paired confidence interval T test results in a P value of 1.105%.

Conclusion

The null hypothesis is assumed to be that the choice of unit converter does not affect the mean time to complete the conversion test. For the paired test, a P value of  0.908% and for the non paired a P value of 1.105% suggested that to a 95% confidence interval the null hypothesis is disproved. This shows a statistically significant difference in the amount of time saved by using the smart units tool. The lower P value on the paired test shows how this difference is especially screen when comparing individual subjects. All but one subject who completed both tests saw an improvement in time using the smart units extension. The one participant who did not see an improvement uniquely struggled with the tool and later found the tool helpful and efficient. Both the median and mean statistics reflect this reduction in time. On average individual participants saw a 166.6s reduction in time to convert 23 varying unit conversions.

Threats to validity
Error could be introduced into this experiment in a variety of ways. First and most prevalent is the relatively small number of participants who took the test. With so few participants and such a high rate of refusal, more participants would be needed to improve the statistical significance of our findings. Additionally some participants found the length of the test daunting and from their feedback was the reason they struggled to finish in a timely manner or dropped out altogether. We also found users getting stuck on a few questions. The way the units were listed made it difficult for participants to correctly get a conversion with the Smart Units tool. For example the tool could recognize “Ton” as a unit but not “Tonnes”. This slowed down many testers. The other factor to consider was which assessment was given first. Some participants may have remembered some of the conversions despite the order of questions being shuffled. This was controlled by having different testers use different tools first.
