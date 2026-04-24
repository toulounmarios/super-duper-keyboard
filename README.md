
helloooooooooooooooooooooo, if you are reading this then you are at the readme section of this repo, so pretty am i right? i know, i know.
im building this project so that i can FINALLY step away from using an old 25 euro gaming keyboard with blue switches ( VERY LOUD ) and make
a compact and aesthetic split keyboad that looks and sounds nice, while also not waking up my entire family at 3am while playing ultrakill or Apex Legends ( both goated btw).
anyways, for anyone who is suprisingly interested in my project here are the key components of the build as well as my key take aways from my first project and some inspo for this.


  first of all, the microcontrollers im using are a pair of seeed xiao nRF52840s, the normal ones will do just fine.
    the pcb was designed on kicad with the libraries from the hackclub stasis event starter project (the split keyboard one) and is manufactured via jlcpcb
   my switches are the kailh choc v2 deep sea silent whale brown switches, due to their tactile yet silent profile.
   for the batteries i havent decided on a li-po battery size for now
  both the case and keycaps ill design after i get the pcb in hand for refernce and ideas 


Now, as for my mistakes, there are afew:
 
 
 &emsp; 1) its best to split the work into chunks and finish them consistently. you dont have to do evrything immidiatly, 
    but try to do related tasks back to back to avoid forgetting where you are at in the build process
 
 
 &emsp; 2) try to simply your models in the pcb editor as much as possible. this is because services like jlcpcb change the shipping 
    and manufacturing costs drastically depending on the size of the pcb, but also stuff like the number of layers on your pcb or the pating and stuff
 
 
 &emsp; 3) thats it for now


my key inspo for this project was the corne layout for split keyboards and the typeractive corn pcb aluminum case for the pcb design



here is the step file of the pcb if you decide to make a custom case for it: [keyboard 1](3d_models/keyboard_1.step)


here is the BOM :

<pre>
Name	                                                        Purpose	                             Qty	Total (USD)	       Link	    Distributor	


Seeed Studio XIAO nRF52840 (XIAO BLE)	             they are the microcontrollers	                  2	    $19.80	          <a href="https://www.seeedstudio.com/Seeed-XIAO-BLE-nRF52840-p-5201.html">link</a>     seeed studio	


0805 806k resistors	                                       for part of vbat	                        100	    $1.68	          <a href="https://www.aliexpress.com/item/1005005184230104.html?spm=a2g0o.productlist.main.1.6249IJXxIJXxPH&algo_pvid=938eadd9-71ba-4352-88da-76219ebfed72&algo_exp_id=938eadd9-71ba-4352-88da-76219ebfed72-0&pdp_ext_f=%7B%22order%22%3A%2216%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&pdp_npi=6%40dis%21EUR%212.25%210.86%21%21%2117.66%216.76%21%402103894417762777976955069ec2d7%2112000032017018112%21sea%21GR%216010249690%21ABX%211%210%21n_tag%3A-29910%3Bd%3A8b9bcfc7%3Bm03_new_user%3A-29895%3BpisId%3A5000000203610259&curPageLogUid=4cgpcI0GnRlD&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005005184230104%7C_p_origin_prod%3A">link</a>    aliexpress	


0805 2M resistors	                                        for the bt pin	                        100	    $2.18	          <a href="https://www.aliexpress.com/item/1005006984056678.html?spm=a2g0o.productlist.main.2.7815aVFfaVFfLN&algo_pvid=960215ef-88d4-41a2-85b6-4be4d2de7d72&algo_exp_id=960215ef-88d4-41a2-85b6-4be4d2de7d72-1&pdp_ext_f=%7B%22order%22%3A%22106%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&pdp_npi=6%40dis%21EUR%211.76%210.86%21%21%2113.79%216.72%21%402103963717762779223528530e0524%2112000038943042424%21sea%21GR%216010249690%21ABX%211%210%21n_tag%3A-29910%3Bd%3A8b9bcfc7%3Bm03_new_user%3A-29895%3BpisId%3A5000000203610259&curPageLogUid=NDv0RorZTDqo&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005006984056678%7C_p_origin_prod%3A">link</a>    aliexpress	

    
1N4148W T4 SOD-123 diodes	                       needed for the keyboard matrix	                100	    $1.84	          <a href="https://www.aliexpress.com/item/1005010653199938.html?spm=a2g0o.detail.pcDetailTopMoreOtherSeller.9.6064rMHVrMHVt1&gps-id=pcDetailTopMoreOtherSeller&scm=1007.40050.354490.0&scm_id=1007.40050.354490.0&scm-url=1007.40050.354490.0&pvid=9ca8f257-295a-4de2-a5ff-3a8f67253366&_t=gps-id:pcDetailTopMoreOtherSeller,scm-url:1007.40050.354490.0,pvid:9ca8f257-295a-4de2-a5ff-3a8f67253366,tpp_buckets:668%232846%238107%231934&pdp_ext_f=%7B%22order%22%3A%221531%22%2C%22eval%22%3A%221%22%2C%22orig_sl_item_id%22%3A%221005010653199938%22%2C%22orig_item_id%22%3A%221005007160563285%22%2C%22sceneId%22%3A%2230050%22%2C%22fromPage%22%3A%22recommend%22%7D&pdp_npi=6%40dis%21EUR%211.34%210.86%21%21%2110.50%216.70%21%40211b612517762807244226998ec4d3%2112000053087454998%21rec%21GR%216010249690%21ABXZ%211%210%21n_tag%3A-29910%3Bd%3A8b9bcfc7%3Bm03_new_user%3A-29895%3BpisId%3A5000000203610259&utparam-url=scene%3ApcDetailTopMoreOtherSeller%7Cquery_from%3A%7Cx_object_id%3A1005010653199938%7C_p_origin_prod%3A1005007160563285">link</a>	  aliexpress	


kailh choc v2 hotswap sockets	                the are the hotswap sockets for my keyswitches	     50	    $5.81	          <a href="https://www.aliexpress.com/item/1005006610506123.html?pdp_npi=4%40dis%21EUR%213.60%211.51%21%21%2129.54%2112.37%21%402141329e17534982253082340d184a%2112000037826084041%21affd%21%21%21&cv=c45834a1-6097-4ce5-bd0a-eecf81d5bb63&gclid=Cj0KCQjwy_fOBhC6ARIsAHKFB79GB903IfZviU8ujcMX8Y--gl5Zxm7TP2JwkSXSLCZnXrenfdEWX5QaAnXwEALw_wcB&aff_fcid=73996a7b7e504db59aeb61aecc68347f-1776206585399-09693&aff_fsk&aff_platform=api-new-product-query&sk&aff_trace_key=73996a7b7e504db59aeb61aecc68347f-1776206585399-09693&terminal_id=88e593aa98a443b1bd172a14f593b1ca&afSmartRedirect=y">link</a>	  aliexpress	


kailh choc v2 deep sea silent mini whale brown	          they are the keyswitches	                 50	   $12.97	          <a href="https://www.aliexpress.com/item/1005008382793794.html?spm=a2g0o.cart.0.0.695838daIfg5m9&mp=1&pdp_npi=6%40dis%21EUR%21EUR%2032.40%21EUR%2010.99%21%21EUR%2010.99%21%21%21%40211b629217762869039837251e1abb%2112000044795077989%21ct%21GR%216010249690%21%211%210%21">link</a>  aliexpress	


the pcb	                                                         its the pcb	                      5	   $15.80	          (jlcpcb wont let me share my cart so youll        jlcpcb
                                                                                                                                 have to do it yourself via their site )	                                                                                                                                              


important notes for ordering and assembly: 

&emsp;1) the resistors for some reason when pressing the link have a different option selected and you'll have to change it yourself in reference to the BOM
&emsp;2) jlcpcb doesnt let you share a link with your cart, so you'll have to go into the jlcpcb site and import the pcb file and then select the options you want, as well as the color of the pcb.
