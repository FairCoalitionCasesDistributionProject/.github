# Welcome To The Fair Division Of Ministries In A Governmental Coalition Calculation System.
## Site URL: https://faircoalitionproj.netlify.app/ <font size="5"> Build Status: [![Netlify Status](https://api.netlify.com/api/v1/badges/cf54cefd-52b3-42de-9a28-65207205a954/deploy-status)](https://app.netlifycom/sites/faircoalitionproj/deploys) </font>


### Table of contents
<ul class="m-0 p-0 list-style-none" data-filterable-for="wiki-pages-filter" data-filterable-type="substring" data-pjax>
        <li class="Box-row">
          <strong><a class="d-block" href="https://github.com/FairCoalitionCasesDistributionProject/FrontEndRelease">Frontend WebGL Release Build Repository</a></strong>
        </li>
        <li class="Box-row">
          <strong><a class="d-block" href="https://github.com/FairCoalitionCasesDistributionProject/ProjectFrontEndThroughUntiy">Frontend Repository (Unity Source Code)</a></strong>
        </li>        
        <li class="Box-row">
          <strong><a class="d-block" href="https://github.com/FairCoalitionCasesDistributionProject/Backend">Backend Source Code Repository With Instructions</a></strong>
        </li>
        <li class="Box-row">
          <strong><a class="d-block" href="https://www.django-rest-framework.org/">The Backend Built Is Based On Django REST Framework</a></strong>
        </li>
        <li class="Box-row">
          <strong><a class="d-block" href="https://github.com/FairCoalitionCasesDistributionProject/Vision1">Vision</a></strong>
        </li>
        <li class="Box-row">
          <strong><a class="d-block" href="https://github.com/FairCoalitionCasesDistributionProject/SRD">SRD</a></strong>
        </li>
        <li class="Box-row">
          <strong><a class="d-block" href="https://github.com/FairCoalitionCasesDistributionProject/SDD">SDD</a></strong>
        </li>
         <li class="Box-row">
          <strong><a class="d-block" href="https://github.com/FairCoalitionCasesDistributionProject/AlgorithmTests">Tests</a></strong>
        </li>
        <li class="Box-row">
          <strong><a class="d-block" href="https://github.com/FairCoalitionCasesDistributionProject/UserFeedbackReply">Feedback</a></strong>
        </li>
    </ul>

[![](http://img.youtube.com/vi/Ap9owYjVAwE/0.jpg)](http://www.youtube.com/watch?v=Ap9owYjVAwE "Fair Distribution Of Ministries In A Coalition (Promo Video).")







## A web application which calculates a fair division of ministries between government coalition members.

The platform gets from each party of a potential coalition, its number of mandates and values for each ministry representing their interest in it as an input. The software returns a fair division of the ministries between the parties as an output accordingly to the leximin criterion.

# So How It Works ?

Here you can try to build a coalition with any parties dividing any ministries you want and see how does it work together.

First, you will be asked to enter the number of ministries that you want to build your coalition on. After that, you will give give those ministries a description (we need to know what are we dividing right ?).

After that, you'll need to tell how many parties there will be in your coalition and how many mandates in total (not only in the coalition) there is. As in the step before, you will be able to give those parties a description.

Please note, the results are highly dependant on the inputs you will use. So, even a difference of a single point might change the division.

Also, after receiving the results, you can copy a URL link which can restore the session for further use.

# The Algorithm

The system is based on an implementation of a linear programming algorithm for fair division of objects between members with non equal rights. The algorithm is based on a theorem that in every division problem between n players with equal rights, exists a proportional division where at most n-1 shared objects.

The algorithm is from Fairpy written by Erel Segal-Halevi

![ 1 ](https://github.com/FairCoalitionCasesDistributionProject/.github/blob/main/profile/Media/1.png)

This function gets the values matrix containing each party's values for each item. It sends to dominating allocation with bounded sharing of the values and a division that each party gets the number of mandates/sum of all the mandates. in this way, we guarantee that each party will get a fair share of their size.

![ 2 ](https://github.com/FairCoalitionCasesDistributionProject/.github/blob/main/profile/Media/2.png)

Here we take an existing allocation and use integer programming to divide the items such that each party will get at least the values it got from the first allocation, however this time only m - 1 item will be shared between the parties.
# Technology
![ 4 ](https://github.com/FairCoalitionCasesDistributionProject/.github/blob/main/profile/Media/4.jpg)

# About Us
![ 5 ](https://github.com/FairCoalitionCasesDistributionProject/.github/blob/main/profile/Media/5.png)










