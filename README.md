# Unit 18 - Pychain Ledger  

![alt="App Image"](media/application-image.png)

## Scenerio  

A Top 5 Bank Fintech Engneer is recently promoted to act as the lead developer on the decentralized finance team. The task to build a blockchain-based ledger system, with a user-friendly web interface. This ledger should allow partner banks to conduct financial transactions (that is, to transfer money between senders and receivers) and to verify the integrity of the data in the ledger.

## Solution

[Click to interact with this Pychain Ledger app](https://unit-18-pychain-ledger.herokuapp.com/)

### The 4 sections that compose Pychain ledger:  

1. Create a Record Data Class

2. Record Date in the Block Data Class

3. Add Relevant User Inputs to the Streamlit Interface

4. Test the PyChain Ledger by Storing Records


### Section 1. Create a Record Data Class

Python data class named `Record`. Give this new class a formalized data structure that consists of the `sender`, `receiver`, and `amount` attributes. To do so, complete the following steps:

* define a new class named `Record`

* add the `@dataclass` decorator immediately before the `Record` class definition

* add an attribute named `sender` of type `str`

* add an attribute named `receiver` of type `str`

* add an attribute named `amount` of type `float`

Note that you’ll use this new `Record` class as the data type of your `record` attribute in the next section.

### Section 2: Modify the Existing Block Data Class to Store Record Data

Rename the `data` attribute in your `Block` class to `record`, and then set it to use an instance of the new `Record` class that you created in the previous section. To do so, complete the following steps:

* in the `Block` class, rename the `data` attribute to `record`

* set the data type of the `record` attribute to `Record`

### Step 3: Add Relevant User Inputs to the Streamlit Interface

Code additional input areas for the user interface of your Streamlit application. Create these input areas to capture the sender, receiver, and amount for each transaction that you’ll store in the `Block` record. To do so, complete the following steps:

* delete the `input_data` variable from the Streamlit interface

* add an input area where you can get a value for `sender` from the user

* add an input area where you can get a value for `receiver` from the user

* add an input area where you can get a value for `amount` from the user

* as part of the “Add Block” button functionality, update `new_block` so that `Block` consists of an attribute named `record`, which is set equal to a `Record` that contains the `sender`, `receiver`, and `amount` values. The updated `Block` should also include the attributes for `creator_id` and `prev_hash`

### Step 4: Test the PyChain Ledger by Storing Records

Test your complete `PyChain` ledger and user interface by running your Streamlit application and storing some mined blocks in your `PyChain` ledger. Then test the blockchain validation process by using your `PyChain` ledger. To do so, complete the following steps:

* in the terminal, navigate to the project folder where you've coded this assignment

* in the terminal, run the Streamlit application by using `streamlit run pychain.py`

* enter values for the sender, receiver, and amount, and then click the Add Block button. Do this several times to store several blocks in the ledger

* verify the block contents and hashes in the Streamlit dropdown menu. Take a screenshot of the Streamlit application page, which should detail a blockchain that consists of multiple blocks. Include the screenshot in the `README.md` file for your GitHub repository.

* test the blockchain validation process by using the web interface. Take a screenshot of the Streamlit application page, which should indicate the validity of the blockchain. Include the screenshot in the `README.md` file for your homework repository

![alt="Section 4"](media/r001-streamlit-section4.png)  
![alt="Steramlit Snow"](media/r002-streamlit-snow.png)

## References

<details><summary>Disclose</summary>  

#### Note  

<sup><a id="ref001">1</a></sup> dataprofessor (2021-06-05). Penguins web app deployed on Heroku. Retrieved from [github.com](https://github.com/dataprofessor/penguins-heroku).

<sup><a id="ref002">2</a></sup> Streamlit.io: st.snow, v1.8.0. Retrieved from [docs.streamlit.io](https://docs.streamlit.io/library/api-reference/status/st.snow).

<sup><a id="ref003">3</a></sup> Gareth Morinan (2021-04-26). 5 ways to customise your Streamlit UI. Retrieved from [towardsdatascience.com](https://towardsdatascience.com/5-ways-to-customise-your-streamlit-ui-e914e458a17c).

<sup><a id="ref004">4</a></sup> Austin Chen (2020-10-08). New layout options for Streamlit. Retrieved from [blog.streamlit.io](https://blog.streamlit.io/introducing-new-layout-options-for-streamlit/).

<sup><a id="ref005">5</a></sup> Fanilo Andrianasolo. Render Static Html With Components. Retrieved from [streamlit-components-tutorial.netlify.app](https://streamlit-components-tutorial.netlify.app/hello-world/static-render/).

<sup><a id="ref006">6</a></sup> Zulko (2022-03-20). MoviePy is a Python library for video editing, can read and write all the most common audio and video formats. Retrieved from [pythonrepo.com](https://pythonrepo.com/repo/Zulko-moviepy-python-video).

<sup><a id="ref007">7</a></sup> Gold, kassius_klay* (2022-03-20). Why does the simplest streamlit example errors out? Retrieved from [stackoverflow.com]](https://stackoverflow.com/questions/71652091/why-does-the-simplest-streamlit-example-errors-out). *If cloud/infrastructure errors-out, change the pinned dependancy to a different version, irrespevtive of the pinned version in the requirments.txt having been a recently working version.

</details>