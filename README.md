AI-Driven Lab Safety Assistant
Final project for the Building AI course.
Summary
The AI-Driven Lab Safety Assistant is a computer vision tool designed for school science laboratories. It uses real-time video analysis to detect if students are wearing proper personal protective equipment (PPE), such as goggles and lab coats, and alerts them of potential hazards. Building AI course project.
Background
In a science high school environment, safety is a priority but accidents often happen due to human error.
• Problem: Students frequently forget to wear goggles or handle chemicals incorrectly.
• Motivation: As a 15-year-old science student, I want to use technology to make school labs safer for everyone.
• Importance: Preventing injuries and ensuring compliance with safety protocols is essential for a productive learning environment.
How is it used?
A camera monitors the lab stations. The AI processes the video feed to identify students and their equipment.
• Environment: School laboratories during practical lessons.
• Users: Students and teachers.
• Alerts: A visual or audio signal (like a red LED) triggers if PPE is missing.
Data sources and AI methods
The project relies on image datasets of PPE (goggles, gloves, coats).
• AI Technique: Computer Vision using Convolutional Neural Networks (CNN) or YOLO.
• Example Code (Logic):
def check_safety(student_image):
    # This is a conceptual example of the detection logic
    has_goggles = detect_object(student_image, "goggles")
    has_lab_coat = detect_object(student_image, "lab_coat")
    
    if not (has_goggles and has_lab_coat):
        return "Safety Warning: Incomplete PPE detected!"
    return "Safety Check Passed: You are ready to experiment."
Challenges
• Privacy: Since this is a school environment, video data must be processed locally and never stored or uploaded to protect student privacy.
• Accuracy: Reflections on glassware or steam from boiling liquids might cause false alerts.
• Ethics: The tool should be seen as a helpful assistant, not as a surveillance system to punish students.
What next?
This project could be expanded to:
1. Detect chemical spills on the floor.
2. Use OCR to read chemical labels and warn if incompatible substances are being mixed.
3. Integrate with smart gas valves to shut off Bunsen burners if a student leaves a station.
Acknowledgments
• Inspired by the safety protocols of my school's science department.
• PPE detection concepts based on open-source datasets and community models.
