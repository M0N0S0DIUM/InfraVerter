SW2 FIX
=======
SW2 has been changed from a 2-pin SPST schematic symbol to a 3-pin SPDT
Nidec CAS-120A symbol matching the existing Button_Switch_SMD:Nidec_Copal_CAS-120A
footprint.

Pin mapping:
  1 = throw used by the circuit
  2 = common used by the circuit
  3 = unused throw (explicitly marked No Connect)

JLC field remains C5962834.

Replace your existing TEST PROJECT.kicad_sch with the file in this folder, reopen
KiCad, then run Tools -> Update PCB from Schematic. The previous warning about
SW2 pad 3 having no corresponding schematic pin should be gone.
