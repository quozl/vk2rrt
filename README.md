# Orana Region Amateur Radio Club Inc, VK2RRT Repeater

## Contacts

* local, Noel VK2ENA,
* near local, Brett VK2WWV,

## History

A limited history of the repeater based on what I've been told or was involved in.

* Albert club handed repeater over to Dubbo club on the understanding that the incorporated Dubbo club would invoice another radio network owner at the site,
* 2006 application to Wireless Institude of Australia (WIA), for [equipment grant](2006-grant-equipment.pdf), total $1000, managed by Brett VK2CBD, linked VK2RRT with VK2RCD and VK2RCC,
* 2007 Australian Amateur Radio Truck Driver's Club funded internet relay linking project, USD $170, proposed by Indy VK2XB,
* 2008-08-09 YHI Power - Neuton Gel 2V 200AH x 6 Batteries $1135.20,
* 2008-10-05 Todae Environmental - 2 x solar panel 90W sunpower $1627.00,
* 2008-10-05 Hagemeyer - 30m 25mm conduit for Boona Mtn $130.00,
* 2008 batteries, charger, and panels installed by Brett VK2CBD, reimbursement for $1032 and $1757,
* 2008 work party, by Brett VK2CBD, Noel VK2ENA, James VK2LQZ, and Petria VK2FERE, trenching cables, clearing, cleaning,
* 2009 license renewal, $62,
* 2009 June, receive antenna bent at right angles,
* 2011-09-26 decommissioning of 70cm link due to relocation of VK2RCD, in turn due to Department of Crown Lands seeking rent and requiring terms and conditions unsustainable for the club,
* 2012 [network diagram](net-diagram.pdf), by Scott VK2UBQ,
* 2013-06-22 work party, by Noel VK2ENA, Bob, Peter, Josh VK2FAXE, James VK2LQZ, and Petria VK2FERE, see [report](2013-06-22-work-party.pdf),
* 2017 work party, Peter VK2BXQ, Noel VK2ENA, battery failure, see [photo #1](images/1.jpg), [photo #2](images/2.jpg),
* 2018-03 [power design review](POWER.md), failure analysis, cost estimates,

## Failure Analysis

* before 2013, repeater audio distorted in low sun or after sunset,
* as of 2013, during charge pack voltage was 12.3 to 12.5 V, at lunch on a sunny day,
    * substantially lower than it should have been,
* as of 2017, one cell cracked, during charge voltage one cell was 1.6 V, discharge on 3 A load was 0.6 V,
* possibly a cell failed, leading to gas release, leading to lower cell voltage, leading to higher charge voltage for other cells, leading to entire pack damage,
* shed has an air vent;
    * so inside air temperature will follow outdoor temperature,
* cells were Neuton Power 2V 200AH supplied by YHI Power,
* are listed at [YHI Power](http://yhipower.com.au/product-1.4.3.html),
* are in their [option brochure](http://yhipower.com.au/data/neutonpower/Neuton%20Power%20Solar%20Battery%20Options.pdf),
* have a [datasheet](http://www.yhipower.com.au/data/neutonpower/ng/NG2-200.pdf),
* should have had a 6000+ cycle life at 20% DoD,
* should have had a designed life of 18 years at room temperature,
* but designed life vs temperature graph in datasheet shows 50&deg;C derating to about 7.5 years,

![Designed Life vs Temperature](images/ng2-200-designed-life-vs-temperature.png)

* so they have also lasted longer than they should have,
* while we could replace one cell, the remaining cells have exceeded their designed life, will fail quickly, and would have to be replaced as well,

## Cost Recovery - Now

* our lease to another radio network owner has provided the needed funds, and the funds are available in our bank account,

## Cost Recovery - Future

* our lease to another radio network owner may have been walked away from, we're still working to verify that,
* other funds arise from annual membership fee of $60,
* we had 17 members last year,
* only one club member is in vicinity of repeater,
* four former members can reach the repeater,

calculations

* yearly budget for replacement of 6 x 2V 200AH batteries;
    * 1135.20 &div; 7.5 = $151.36
* at least three club members needed, excluding insurances;
    * 60 &times; 3 = $180

## Diagram

rx omni --> 2m rx --> 200m long cable --> controller

controller --> 2m tx --> cavity filter --> tx omni

yagi --> 70cm rx --> controller

controller --> 70cm tx --> yagi

## Other References

* [VK2CA's VK2 repeater map](http://vkham.com/maps/vk-repeaters/vk1-vk2-repeaters) and entry for [VK2RRT](http://www.vkham.com/Repeater/condobolin.html)
* [Australian Communications and Media Authority License Number 2622/1](https://web.acma.gov.au/rrl/licence_search.licence_lookup?pLICENCE_NO=2622/1)
