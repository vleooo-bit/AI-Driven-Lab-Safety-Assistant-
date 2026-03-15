# AI-Driven Lab Safety Assistant

Final project for the Building AI course.

## Summary
The **AI-Driven Lab Safety Assistant** is a computer vision tool designed for school science laboratories. It uses real-time video analysis to detect if students are wearing proper personal protective equipment (PPE), such as goggles and lab coats, and alerts them of potential hazards.

## Background
In a science high school environment, safety is a priority but accidents often happen due to human error. 
* **Problem:** Students frequently forget to wear goggles or handle chemicals incorrectly.
* **Motivation:** As a 15-year-old science student, I want to use technology to make school labs safer for everyone.
* **Importance:** Preventing injuries and ensuring compliance with safety protocols.

## How is it used?
A camera monitors the lab stations. The AI processes the video feed to identify students and their equipment.
* **Environment:** School laboratories during practical lessons.
* **Users:** Students and teachers.
* **Alerts:** A visual or audio signal triggers if PPE is missing.

## Data sources and AI methods
The project relies on image datasets of PPE (goggles, gloves, coats).
* **AI Technique:** Computer Vision using Convolutional Neural Networks (CNN).
* **Example Code (Logic):**

```python
def check_safety(https://www.dpi-dm.it/dispositivi-di-protezione-individuale-dpi/):
    # Pseudocode for PPE detection
    has_goggles = detect_object(https://www.camiciedivise.it/occhiali-protettivi-laboratorio.html)
    has_lab_coat = detect_object(https://www.bazzacco.it/shop/laboratorio-chimica/46-camice-laboratorio-chimica.html)
    
    if not (has_goggles and has_lab_coat):
        return "Safety Warning: Incomplete PPE!"
    return "Safety Check Passed"

