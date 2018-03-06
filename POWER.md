# Draft Power Budget for VK2RRT

by James Cameron VK2LQZ<br>
6th March 2018


## Equipment Measurements

Received by e-mail and telephone conversation with Peter VK2BXQ.

* VHF receiver, 125 mA idle, 250 mA receive,
* VHF transmitter, 120 mA idle,
* repeater controller, 25 mA,
* UHF receiver and transmitter, 400 mA; note link with VK2RCD is blocked by terrain so this equipment will be off,
* solar regulator, 60 mA,
* two 90 W solar panels, total 180 W,
* wired in series at the moment.

## Generation Estimates

* assume nominal five hours insolation,
* total 900 WH per day, (180 &times; 5),

## Consumption Estimates

* idle current 0.33 A, 4.75 W, 114 WH per day,
* transmit current unknown, license limit 120 W, assume one hour per day, 120 WH per day,
* total 230 WH per day,

## Worst Case - No Sun

* check that there is capacity to cover multiple days overcast,
* typically 33% insolation; generation of 300 WH, consumption of 230 WH, plus losses,
* generation during overcast is sufficient to meet consumption assuming at least 230 WH of battery storage,
* generation on sunny days is more than three times consumption.

## Purchases recommended by Peter VK2BXQ and Brett VK2WWV,

* [Giant 12V 130AH AGM Deep Cycle Battery](https://www.aussiebatteries.com.au/batteries/deep-cycle-agm/130ah-12v-agm-deep-cycle-battery) (aussiebatteries.com.au)
    * $289 each, quantity 3, quoted total $810,
    * Maximum temperature 40&deg;C,
    * Weight 31 kg each,

  calculations and review by James VK2LQZ,

    * Usable capacity at 10% DoD; 39 AH, 539 WH per day, 5 years, (not specified by retailer),
    * Battery life will be reduced by up to 50% due to temperature,
    * Emergency capacity 390 AH, 5382 WH, or 21 days with solar array down,
    * Battery life will be reduced by up to 90% if emergency capacity is ever used,
    * Meets requirements, but will have a short life due to temperature.

* [EPSOLAR Tracer4215BN MPPT charge controller](http://www.epsolarpv.com/en/index.php/Product/pro_content/id/573/am_id/136) (epsolarpv.com)

    * Already purchased as a donation by Peter,
    * Enclosure IP30,
    * Maximum temperature 55&deg;C,
    * Maximum input power 520 W,
    * Maximum charge current 40 A,
    * Low voltage cutoff 11.1 V,
    * Low voltage reconnect 12.6 V,

  calculations and review by James VK2LQZ,

    * Charge current at 180 W input with battery at 11.1 V; 16 A,
    * Meets requirements,

* Solar panels

    * Total of 400W,
    * Adapt frame for different panels, completed,
    * Fix frame to ground,
    * Retire existing panels,
    * Exceeds requirements,

  calculations and review by James VK2LQZ,

    * Is not required, there is three times the power now,
    * System will complete charging earlier in the day, lowering the peak battery temperature slightly,
    * Panels will be idle most of the day.

## Purchases recommended by James VK2LQZ

* [Sentry 40AH 12V](https://www.rpc.com.au/catalog/sentry-lithium-battery-40ah-12v-p-4588.html) (rpc.com.au)

    * $645,
    * Maximum temperature 50&deg;C,
    * Minimum temperature -20&deg;C,
    * Weight 5.5kg,
    * Maximum charge current 40A,
    * Contains a charge balancing battery management system,
    * [Datasheet](https://www.rpc.com.au/pdf/sentry_12V40S_datasheet.pdf),

  calculations,

    * Usable capacity at 100% DoD; 40AH, 552 WH per day, 5.5 years,
    * Emergency capacity same, or two days,
    * Meets requirements.

* Solar panel

    * not required; power budget is sufficient with UHF link disconnected.

* [Victron SmartSolar MPPT Regulator 75/15](https://www.rpc.com.au/catalog/victron-smartsolar-mppt-regulator-75v-15a-p-4624.html) (rpc.com.au)

    * $186,
    * Enclosure IP43,
    * Maximum temperature 60&deg;C,
    * Maximum input power 440 W,
    * Maximum charge current 15 A,
    * Low voltage cutoff 11.1 V,
    * Low voltage reconnect 13.1 V,
    * [Datasheet](https://www.rpc.com.au/pdf/victron_SmartSolar_MPPT_75-100_10-20_datasheet.pdf).

  calculations,

    * Charge current at 180 W input with battery at 11.1 V; 15 A;

## Risks

* panels may have been damaged, suggested by David VK2AYO; panel output should be checked, adding series panels will not help if one of the panels is damaged,
* adding series panels of different power won't be tracked properly by the MPPT control algorithm, suggested by James VK2LQZ,
* cable length of 35m does not seem right, trench was much shorter, suggested by Petria VK2FERE, see photograph,
* temperature can exceed 40&deg;C in shed; previous battery had enough thermal mass to avoid damage, but a small-celled AGM battery may not escape this.

----
