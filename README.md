# Voron V0/V0.1-Servo-Activated-Microswitch-Probe

Now the cute little printer has auto bed mesh levelling and screw tilt adjust!!! 
This applicable to Voron V0/V0.1

This is a remix of these https://www.thingiverse.com/thing:5026392 and https://github.com/oldfar-t/Side-Swipe-Magnetic-Probe.

I did not like losing some 10mm on Y axis in the Side Swipe and the mount IMHO ruins the look of the miniAB. As of the Sherpa Klicky Probe, I dont like it is being so close to the bed, as it can be picked up by the printhead while printing. So I remix them and made a mod of the miniAB. 

BOM:
- 2 - M3x8 BHCS or SHCS Bolts 
- 2 - M3 Nuts
- 5/6 - 6mmx3mm Neodymium Magnets
- 1 - [Omron Mouse Microswitch](https://www.amazon.com/dp/B00HPL57JQ/?coliid=I2L344Q2DNJEAU&colid=WW0P09PQO065&psc=1&ref_=lv_ov_lig_dp_it)
- 1 - [MG90s Hobby Metal Gear Servo Motor](https://www.amazon.com/Maxmoral-Upgraded-Digital-Vehicle-Helicopter/dp/B07NV476P7/ref=pd_lpo_1?pd_rd_i=B07NV476P7&psc=1)
- 1 - [300mm Servo Extension Cable](https://www.amazon.com/gp/product/B01LA9YDEI/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1)
- 1 - 450mm Two conductor wire 24AWG or 28AWG

## Change this in the printer.cfg
[include probe.cfg]

[stepper_z]
endstop_pin: probe:z_virtual_endstop #default PC2 for home with Z endstop, Use "probe:z_virtual_endstop" if you want to home with probe

;position_endstop

position_min: -15

## Wiring
See Diagram

## Tips
You need to align the servo with the probe to the miniAB mount so that it will slide in/out properly.

You may need to make the holes on the probe a little bit bigger so the soldered conductor on the microswitch can fit into the hole.

I put a dab of CA glue to the microswitch so that it will not move.

## Notes
I dont knnow how to use CAD or design my own, I just remix/cut the two designs I mentioned. So, may this thing help other designers to perfect it it the future
