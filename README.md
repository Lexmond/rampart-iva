# rampart-iva
RAMPART protocol folder for Influenza A virus

## Installing
Clone this repository:

```
git clone https://github.com/artic-network/rampart-iva.git
```

Create conda environment and activate it:

```
cd rampart-artic
conda env create -f environment.yml
conda activate rampart-artic
```

## Running

Create run folder:

```
mkdir [run_name]
cd [run_name]
```

Where `[run_name]` is whatever you are calling todays run (as specified in MinKNOW).

Run RAMPART (assuming the `rampart-nipah` directory is next to `[run_name]`):

```
rampart --protocol ../rampart-iva/protocol --basecalledPath ~/MinKNOW/data/reads/[run_name]/pass
```

`basecalledPath` should be set to whereever MinKNOW/guppy is going to write its basecalled files.

## Example Data

The directory `example_data` contains some reads from an influenza virus MinION run to test RAMPART with. To try this:

```
cd rampart/example_data
rampart --protocol ../protocol 
```

The `run_configuration.json` file contains the settings for running this example data.

Open a browser to view [http://localhost:3000](http://localhost:3000)
