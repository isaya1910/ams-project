# ams-project

// содержит информацию в себе по дате проведения, материалу и длительности
Lesson: 
  startTime(): DateTime
  duration(): Duration
  matherial(): Matherial
  

// содержит себе данные по прошедшим и будущим курсам, может относится как к студенту так и к преподавателю  
Course:
  futureLessons(): List<Lesson>
  endedLessons(): List<Lesson>
  nextLesson(): Lesson
  
   
// содержит в себе информацию по оставшимся занятиям и дату окончания студента
Abonnement:
  balance(): Balance()
  endDate(): Date
  
// содержит в себе информацию по посещению урока студентами
Lesson Attendance:
  students(): List<Student
  participatedStudents():  List<Student>
  missedStudents(): List<Student>

// может отпроситься с урока, поставить абонемент на паузу
Student:
  requestLessonSkip(lesson: Lesson)
  requestAbonementPause()
  
// на начальном этапе может проставлять аттенданс и ставить бонусы  
Teacher: 
  markAttendence(student: Student, lesson: Lesson)
  giveBonus(student: Student)

Admin: 
  createCourse()
  acceptLessonSkip()
  declineLessonSkip()
  acceptCoursePause()
  declineCoursePause()
  rescheduleLesson()
