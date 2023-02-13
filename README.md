# PyChain Ledger

![alt=""](Images/application-image.png)

In this challenge, I build a blockchain-based ledger system, complete with a user-friendly web interface. The blockchain has transactions features (that is, to transfer money between senders and receivers) and to verify the integrity of the data in the ledger.

## Instructions

1. create the `PyChain` ledger includes the functionality to create blocks, perform the proof of work consensus protocol, and validate blocks in the chain.

2.Create a blueprint for the financial transaction records that the blocks of the ledger will store.

3. Add Relevant User Inputs to the Streamlit interface.

4. last is to Test the PyChain Ledger by Storing Records.

---

The steps are divided into the following sections:

1. Create a Record Data Class

2. create a Block Data Class to Store Record Data

3. Add Relevant User Inputs to the Streamlit Interface

4. Test the PyChain Ledger by Storing Records

### Step 1: Create a Record Data Class by completing the following steps:

1. Define a new class named `Record`.

2. Add the `@dataclass` decorator immediately before the `Record` class definition.

3. Add an attribute named `sender` of type `str`.

4. Add an attribute named `receiver` of type `str`.

5. Add an attribute named `amount` of type `float`.


### Step 2: create a Block Data Class to Store Record Data

Rename the `data` attribute in `Block` class to `record`, and then set it to use an instance of the new `Record` class that I created in the previous section. 

steps to complete are:

1. rename the `data` attribute to `record`.

2. Set the data type of the `record` attribute to `Record`.

### Step 3: Add Relevant User Inputs to the Streamlit Interface

Code additional input areas for the user interface of my Streamlit application. Create these input areas to capture the sender, receiver, and amount for each transaction that I’ll store in the `Block` record. To do so, I completed the following steps:

1. Delete the `input_data` variable from the Streamlit interface.

2. Add an input area where I can get a value for `sender` from the user.

3. Add an input area where I can get a value for `receiver` from the user.

4. Add an input area where I can get a value for `amount` from the user.

5. As part of the “Add Block” button functionality, update `new_block` so that `Block` consists of an attribute named `record`, which is set equal to a `Record` that contains the `sender`, `receiver`, and `amount` values. The updated `Block` should also include the attributes for `creator_id` and `prev_hash`.

### Step 4: Test the PyChain Ledger by Storing Records

Test my complete `PyChain` ledger and user interface by running my Streamlit application and storing some mined blocks in my `PyChain` ledger. Then test the blockchain validation process by using my `PyChain` ledger. I should have use terminal but it is unfortunate that I couldn't run streamlit using terminal but I used `Gitpod code`

But if use terminal, then this are the steps :

1. In the terminal, navigate to the project folder to access this file.

2. In the terminal, run the Streamlit application by using `streamlit run pychain.py`.

3. to test the streamlit, Enter values for the sender, receiver, and amount, and then click the Add Block button.

4. Verify the block contents and hashes in the Streamlit dropdown menu. 

