# Progetto CCAR
	
## Regolazione Trascrizionale

***
Autore:
* Lorenzo Pagliara <l.pagliara5@studenti.unisa.it>

***
### Organizzazione cartella
La cartella del progetto è organizzata nel modo seguente:

|File|Descrizione| 
|:---:|:---:| 
|`./transcriptional_regulation.mlx`| É il file principale per l'esecuzione di tutte le simulazioni.|
|`./Phase_Portrait/TranscriptionalRegulation.mat`| É il file contenente la configurazione del plugin Phase Plane per ottenere il diagramma di fase del sistema in esame.|
|`./Simulink/transcriptional_regulation.slx`| É il file Simulink contenente l'intero schema di retroazione del sistema, che consente di effettuare lo switch del controllore mediante comando dal workspace.|
|`./Simulink/transcriptional_regulation_observer.slx`| É il file Simulink contenente l'intero schema di retroazione del sistema, con integrato l'osservatore.|
|`./Simulink/transcriptional_regulation_kalman_filter.slx`| É il file Simulink contenente l'intero schema di retroazione del sistema, con integrato il filtro di Kalman.|
|`./Simulink/transcriptional_regulation_model.mlx`| É il file contenente la funzione Matlab che implementa il modello matematico del sistema.|
|`./Simulink/transcriptional_regulation_fbl_controller.mlx`| É il file contenente la funzione Matlab che implementa il controllore non lineare del sistema.|

***
### Come eseguire
#### Script principale
Prima di eseguire lo script Matlab contenuto nel file `./transcriptional_regulation.mlx` occorre aggiungere al path di Matlab la cartella `Simulink`:

> da Matlab tasto destro sulla cartella `Simulink` e selezionare `Add to Path -> Selected Folders and Subfolders`.

***

#### Diagramma di fase
Per visualizzare il diagramma di fase del sistema:

1. scaricare [PhasePlane](https://it.mathworks.com/matlabcentral/fileexchange/91705-phase-plane-and-slope-field-apps?s_tid=srchtitle_Phase%2520Plane_2);
2. avviare PhasePlane da Apps;
3. caricare il sistema da `Custom library -> load` e caricare il file `./Phase_Portrait/TranscriptionalRegulation.mat`;
4. impostare i parametri del sistema `Custom library -> RegolazioneTrascrizionale`.



