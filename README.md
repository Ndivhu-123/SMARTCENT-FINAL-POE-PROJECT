# SMARTCENT-FINAL-POE-PROJECT
SmartCent is a personal budgeting Android app prototype built with Kotlin and RoomDB. It helps users track expenses, manage categories, and visualize spending through a clean, themed UI. The project showcases applied skills in mobile development, database integration, and professional design.
# SmartCent – Personal Finance and Budgeting Application

## Overview

SmartCent is an Android-based personal finance management application designed to help users develop better budgeting habits, track their spending, and improve their financial literacy. The app combines expense tracking, income management, goal setting, progress monitoring, and educational content into a single user-friendly platform.

The primary objective of SmartCent is to empower users to take control of their finances by providing real-time insights into their spending patterns, budget performance, and financial goals.

---

## Features

### User Profile

Users can create and manage their personal profile, including their name and profile picture. Profile information is stored using SharedPreferences, ensuring data persists across application sessions.

### Dashboard

The dashboard serves as the central hub of the application and provides quick access to all major features, including:

* Add Expense
* Add Income
* Set Budget Goals
* View Reports
* Budget Progress
* Expense Categories

The dashboard also displays summary cards showing important financial information such as total income, total expenses, budget goals, and monthly spending.

### Expense Management

Users can record expenses by entering:

* Date
* Time
* Description
* Category
* Amount

To improve record keeping, expenses can also include receipt photographs, making it easier to track and verify spending.

### Income Management

Users can record income transactions with details such as:

* Date
* Description
* Amount

All income entries are securely stored in the local SQLite database and contribute to financial summaries and reports.

### Expense Categories

SmartCent allows users to organize expenses into categories such as:

* Food
* Transport
* Entertainment
* Shopping
* Utilities

Categorization helps users better understand spending habits and improves report accuracy.

### Budget Goals

Users can create budget goals by setting:

* Minimum Budget Goal
* Maximum Budget Goal

These values are stored in the database and used to calculate spending progress and budget performance.

### Budget Progress Tracking

SmartCent provides a visual representation of budget performance through a progress bar.

The application retrieves financial information using database methods:

* `getTotalIncome(userId)`
* `getTotalExpenses(userId)`
* `getBudgetGoal(userId)`
* `getBudgetMax(userId)`

#### Progress Calculation

The application calculates budget usage using the formula:

Progress Percentage = (Total Expenses ÷ Budget Goal) × 100

The resulting percentage is displayed through:

* A horizontal progress bar
* Percentage indicators
* Text-based feedback

This allows users to quickly determine whether they are staying within budget.

### Monthly Expense Tracking

SmartCent automatically calculates the total expenses incurred during the current month.

#### How It Works

The application:

1. Determines the start and end dates of the current month.
2. Queries the database for expenses recorded within that date range.
3. Calculates the total monthly expenditure.
4. Displays the result on the dashboard.

This feature helps users monitor spending trends and identify periods of high expenditure.

### Reports and Analysis

Users can generate reports based on recorded expenses and income. These reports provide insights into:

* Spending habits
* Category-based expenditure
* Budget performance
* Financial trends

### Gamification System

To encourage consistent financial management, SmartCent includes a gamification system.

Users can unlock:

* Achievement Badges
* Milestone Rewards
* Progress Recognition

Achievements are earned by:

* Recording expenses
* Recording income
* Reaching savings goals
* Maintaining budgeting consistency

This feature helps increase engagement and motivation.
The additional features 
### Budgeting Course and Assessment

SmartCent includes an interactive Budgeting Course designed to improve users' financial literacy and budgeting knowledge. The course provides educational content that teaches users about responsible spending, saving strategies, goal setting, and effective money management practices.

#### How It Works

* Users can access the budgeting course through the Study Mode section.
* The course presents budgeting concepts in an easy-to-understand format.
* Educational material is structured into learning sections that guide users through important financial topics.
* Users can study at their own pace while actively applying the concepts within the SmartCent application.

#### Budgeting Knowledge Test

To reinforce learning, SmartCent includes a budgeting assessment quiz.

The quiz:

* Contains multiple-choice budgeting questions.
* Tests users' understanding of financial concepts covered in the course.
* Provides immediate feedback on answers.
* Encourages users to improve their financial decision-making skills.
* Can be retaken to improve knowledge and track learning progress.

This feature transforms SmartCent from a simple budgeting application into an educational platform that helps users develop long-term financial management skills.

---

### Financial Literacy Video Tutorials

SmartCent integrates educational YouTube budgeting tutorials to provide users with additional learning resources.

#### How It Works

* Users can access a curated collection of budgeting and personal finance videos directly within the application.
* Each tutorial focuses on important financial topics such as:

  * Budget Planning
  * Saving Strategies
  * Debt Management
  * Financial Goal Setting
  * Smart Spending Habits
* When a user selects a tutorial, the application opens the video using an external YouTube link or video intent.
* Users can watch expert-led financial literacy content without having to search for resources independently.

#### Benefits

* Supports visual and self-paced learning.
* Reinforces concepts taught in the budgeting course.
* Provides practical real-world financial advice.
* Enhances user engagement and financial awareness.

By combining budgeting tools, educational courses, assessments, and video-based learning, SmartCent promotes both financial management and financial literacy, helping users make informed financial decisions and build sustainable money habits.


### Study Mode

SmartCent promotes financial literacy through an integrated educational section called Study Mode.

Study Mode includes:

* Budgeting tutorials
* Educational videos
* Interactive quizzes
* Personal finance learning resources

This allows users to improve their financial knowledge while actively managing their finances.

---

## Technologies Used

* Kotlin
* Android Studio
* SQLite Database
* SharedPreferences
* Material Design Components
* Android Jetpack Libraries

---

## Data Storage

SmartCent uses two primary storage mechanisms:

### SQLite Database

Used for storing:

* Users
* Expenses
* Income
* Categories
* Budget Goals

### SharedPreferences

Used for storing:

* User profile information
* Profile images
* Login session information

---

## Project Objective

The goal of SmartCent is to provide an accessible and engaging financial management solution that helps users:

* Track income and expenses
* Create realistic budgets
* Monitor financial progress
* Improve spending habits
* Learn essential financial literacy skills

By combining budgeting tools with educational content and gamification, SmartCent offers a comprehensive platform for achieving better financial well-being.

