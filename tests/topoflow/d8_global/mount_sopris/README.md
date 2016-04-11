## Create and run the test

    model_id=$(wmt model save d8_global.yaml)
    wmt model upload $model_id Mount_Sopris.rti
    wmt model upload $model_id Mount_Sopris_DEM.rtg
    sim_id=$(wmt simulation save $model_id D8_Testing_Mount_Sopris)
    wmt simulation launch $sim_id
