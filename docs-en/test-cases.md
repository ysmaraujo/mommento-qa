### Test Scenario: Start Pomodoro timer

**Test Case ID:** TC-01  
**Title:** Verify that the Pomodoro timer starts and runs correctly until completion  

**Preconditions:**  
- User has accessed https://www.mommento.com.br  
- Timer is in the initial state (25 minutes)  
- No active session is running  

**Test Steps:**
1. Click on the "Iniciar" button  
2. Observe if the timer starts counting down  
3. Wait until the timer reaches 00:00  

**Test Data:**  
N/A  

**Expected Result:**
- The timer starts counting down from 25 minutes  
- The "Iniciar" button changes to "Pausar"  
- The timer continues decreasing correctly until 00:00  
- When the timer reaches 00:00 :
  - A sound alarm is triggered  
  - The phrase changes from focus to break  
  - One indicator dot becomes fully visible  
  - The timer automatically switches to break time (5 minutes)

  ---

  ### Test Scenario: Pause Pomodoro timer

**Test Case ID:** TC-02  
**Title:** Verify that the Pomodoro timer pauses correctly when clicking the "Pausar" button  

**Preconditions:**  
- User has started the Pomodoro timer  
- Timer is currently running  

**Test Steps:**
1. Click on the "Pausar" button  
2. Observe the timer value  
3. Wait a few seconds to confirm if the timer remains unchanged  

**Test Data:**  
N/A  

**Expected Result:**
- The timer stops decreasing  
- The timer value remains the same after pausing  
- The "Pausar" button changes to "Continuar"  
- The user is able to resume the timer after pausing

---

### Test Scenario: Reset Pomodoro timer

**Test Case ID:** TC-03  
**Title:** Verify that the Pomodoro timer resets correctly when clicking the "Resetar Timer" button  

**Preconditions:**  
- User has started the Pomodoro timer  
- Timer is currently running or paused  

**Test Steps:**
1. Click on the "Resetar Timer" button  
2. Observe the timer value  
3. Verify if the timer stops running  

**Test Data:**  
N/A  

**Expected Result:**
- The timer resets to the initial value (25 minutes in focus mode or 5 minutes in break mode)  
- The timer stops running after reset  
- The "Pausar" button changes to "Iniciar"  
- The timer does not continue counting after reset

---

### Test Scenario: Switch between focus and break modes

**Test Case ID:** TC-04  
**Title:** Verify that the Pomodoro timer switches correctly when clicking the "Trocar Modo" button  

**Preconditions:**  
- User has accessed https://www.mommento.com.br  
- Timer is in the initial state (focus mode - 25 minutes)  
- No active session is running  

**Test Steps:**
1. Click on the "Trocar Modo" button  
2. Observe the timer value  
3. Observe the phrase displayed on the screen  

**Test Data:**  
N/A  

**Expected Result:**
- The timer switches from focus mode (25 minutes) to break mode (5 minutes), or vice versa  
- The displayed time updates accordingly  
- The phrase changes according to the selected mode (focus or break)  
- The timer does not start automatically after switching modes

---

### Test Scenario: Pomodoro timer completes and triggers alarm

**Test Case ID:** TC-05  
**Title:** Verify that an alarm is triggered and the timer transitions correctly when reaching 00:00  

**Preconditions:**  
- User has started the Pomodoro timer  
- Timer is currently running in focus mode  

**Test Steps:**
1. Click on the "Começar" button (if not already started)  
2. Wait until the timer reaches 00:00  
3. Observe the system behavior when the timer completes  

**Test Data:**  
N/A  

**Expected Result:**
- An alarm sound is triggered when the timer reaches 00:00  
- The focus phrase changes to the break phrase  
- The timer automatically switches to break mode (5 minutes)  
- The control button changes to "Começar"  
- One Pomodoro cycle indicator (dot) becomes fully active  

---

### Test Scenario: Long break after 4 Pomodoro cycles

**Test Case ID:** TC-06  
**Title:** Verify that a long break (15 minutes) is triggered after completing 4 Pomodoro cycles  

**Preconditions:**  
- User has completed 3 Pomodoro cycles  
- The 4th Pomodoro cycle is currently running in focus mode  

**Test Steps:**
1. Wait until the timer reaches 00:00 in the 4th Pomodoro cycle  
2. Observe the timer behavior after completion  

**Test Data:**  
N/A  

**Expected Result:**
- The timer switches to a long break of 15:00 minutes  
- All 4 Pomodoro indicator dots are active  
- The phrase changes to break mode  
- The control button changes to "Iniciar"

### Test Scenario: Break timer completes and returns to focus mode

**Test Case ID:** TC-07  
**Title:** Verify that the timer switches from break mode to focus mode after completion  

**Preconditions:**  
- The Pomodoro timer is currently running in break mode  
- A break session is in progress  

**Test Steps:**
1. Wait until the timer reaches 00:00  
2. Observe the system behavior after the break ends  

**Test Data:**  
N/A  

**Expected Result:**
- The timer switches to focus mode (25 minutes)  
- The displayed time resets to 25:00  
- The phrase changes to focus mode  
- The control button is set to "Iniciar"  

---

### Test Scenario: Create a new task

**Test Case ID:** TC-08  
**Title:** Verify that a new task can be successfully created  

**Preconditions:**  
- User is on the main application screen  
- The task sidebar is accessible  

**Test Steps:**
1. Click on the "+" button to open the task sidebar  
2. Enter a task name in the input field  
3. Click on the "Adicionar tarefa" button  
4. Verify if the task appears in the task list  

**Test Data:**  
N/A  

**Expected Result:**
- The new task is added to the task list  
- The task appears under pending tasks  
- The task name matches the input provided  

---

### Test Scenario: Set a task as active

**Test Case ID:** TC-09  
**Title:** Verify that a task can be set as active and linked to the Pomodoro timer  

**Preconditions:**  
- User is on the main application screen  
- At least one task exists in the task list  
- The task sidebar is open  

**Test Steps:**
1. Locate an existing task in the task list  
2. Click on the task selection control  
3. Observe the task state and UI changes  

**Test Data:**  
N/A  

**Expected Result:**
- The selected task is marked as active  
- The task is visually highlighted as active  
- Only one task can be active at a time (if applicable)  
- The active task is displayed in the main screen under the timer  
- The Pomodoro timer associates focus time with the active task  

---

### Test Scenario: Set a task as active

**Test Case ID:** TC-09  
**Title:** Verify that a task can be set as active and correctly linked to the Pomodoro timer  

**Preconditions:**  
- User is on the main application screen  
- At least one task exists in the task list  
- The task sidebar is open  

**Test Steps:**
1. Locate an existing task in the task list  
2. Click on the task card (not the checkbox)  
3. Observe the task state and UI changes  
4. Check the main screen above the timer  

**Test Data:**  
N/A  

**Expected Result:**
- The selected task is marked as active  
- The task card is highlighted with a border matching the selected theme color  
- The task appears above the timer on the main screen  
- Only one task can be active at a time (if applicable)  
- The Pomodoro timer associates focus time with the active task  

---

### Test Scenario: Complete Pomodoro linked to active task

**Test Case ID:** TC-10  
**Title:** Verify that completing a Pomodoro updates the active task statistics  

**Preconditions:**  
- User has an active task selected  
- Pomodoro timer is running in focus mode  

**Test Steps:**
1. Wait until the Pomodoro timer reaches 00:00  
2. Observe the active task in the sidebar  
3. Check the task details below the task name  

**Test Data:**  
N/A  

**Expected Result:**
- The completed Pomodoro is counted for the active task  
- A clock icon appears below the task name  
- The number of Pomodoros completed is displayed correctly (e.g., "13 pomodoros")

---

### Test Scenario: Mark task as completed using checkbox

**Test Case ID:** TC-11  
**Title:** Verify that clicking the checkbox marks the task as completed  

**Preconditions:**  
- At least one task exists in the task list  

**Test Steps:**
1. Locate an existing task  
2. Click on the checkbox of the task  
3. Observe the task status  

**Test Data:**  
N/A  

**Expected Result:**
- The task is marked as completed  
- The task moves to the completed tasks section  
- The task is no longer active  

