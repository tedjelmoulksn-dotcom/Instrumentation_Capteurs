# Sensor Characterization and Conditioning

MATLAB experiments relating physical quantities to sensor resistance or output voltage. The scripts combine recorded measurements, characteristic curves and conditioning calculations for temperature and displacement sensing.

![Instrumentation Capteurs project overview](assets/project-overview.svg)

*Technical study overview based on the available repository material.*

## Studies

| Script in [src](src/) | Measurement or circuit |
| --- | --- |
| `ctn_resistance_temperature.m` | NTC resistance versus temperature |
| `ctn_pont_diviseur.m` | Voltage-divider response for an NTC sensor |
| `ctn_conditionnement.m` | Temperature-sensor signal conditioning |
| `pt100_resistance_temperature.m` | Platinum RTD resistance characteristic |
| `lvdt_caracteristique.m` | LVDT voltage versus displacement |

These exercises connect sensor behaviour to the electrical signal an acquisition system receives. The MATLAB arrays contain the measurements used by each study; they are not live device interfaces.

## Run a study

Open a script in MATLAB and run it independently. Inspect the measurement vectors, units and circuit parameters before comparing curves or changing the experiment.

For the LVDT study, distinguish the measured series from the linear reference model in the source. Its plotting commands can replace earlier curves, so the displayed figure alone does not represent every recorded series.

## Related work

[Instrumentation Physique](https://github.com/tedjelmoulksn-dotcom/Instrumentation_Physique) contains measurement reports; [LabVIEW Instrumentation](https://github.com/tedjelmoulksn-dotcom/LabVIEW_Instrumentation) contains graphical acquisition exercises.
