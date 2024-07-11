Interview Preparation - 2
Mon, Jul 8, 2024
7:30pm - 8:41pm

Meeting Report and Record Link:
https://app.read.ai/analytics/meetings/01J29ABEG3G0W4FCA0HWNPKXHR

Summary:

The meeting was led by Zakeer Hussain Syed, who covered a range of topics related to website development and responsive design. He engaged participants in discussions on HTML form validation, CSS reset, image accept ratios, image sizing and positioning, centering images, and centering elements using CSS properties. Throughout the meeting, Zakeer encouraged participants to share their progress, approach, and choice of technology stack in creating their websites, while actively involving them in the discussions.

Zakeer provided detailed explanations on various topics, including the use of the required attribute and custom validation in HTML form validation, the significance of CSS reset in maintaining uniform styling across various browsers and devices, and the intricacies of image accept ratios and their impact on fitting images. He also explored various techniques and properties for centering images and elements, including the use of percentages and the transform property.

The meeting was interactive, with participants contributing to the discussions and seeking clarification on various topics. Zakeer emphasized the importance of understanding the principles behind the topics covered and encouraged participants to ask questions. The meeting concluded with Zakeer expressing gratitude and announcing the continuation of the session the following day.


Chapters & Topics:

Discussion on Website Development and Responsive Design
Zakeer Hussain Syed initiates a discussion on website development and responsive design, seeking input from participants on their progress and approach in creating their websites. He also asks about their choice of technology stack and whether they have worked on responsive design, encouraging them to share details and explain their reasoning.

HTML Form Validation and Custom Validation
Zakeer Hussain Syed leads a discussion on HTML form validation, emphasizing the use of the required attribute and the need for custom validation in certain scenarios. He highlights the importance of allowing form submission without validation and suggests using the novalidate attribute to achieve this. The team engages in a dialogue about the implications and limitations of HTML inbuilt validations and the role of JavaScript in form validation.

Discussion on HTML and CSS Reset
Zakeer Hussain Syed leads a discussion on the necessity of adding rows and the concept of CSS reset in web development. He emphasizes the importance of maintaining standard styling and demonstrates the use of an HTML validator to ensure proper structure. Haseena Mohammad expresses confusion, prompting further clarification on the topic.
* HTML Validation

Importance of CSS Reset
Zakeer Hussain Syed discusses the necessity of CSS reset to achieve consistent styling across different browsers and devices. He illustrates how default browser styles can cause inconsistencies and demonstrates the use of CSS reset to address these issues, emphasizing the importance of including it in new projects.
* CSS Reset
* Responsive Design

Image Accept Ratios and Fitting Options
Zakeer Hussain Syed provides a detailed explanation of image accept ratios, including examples such as 3-2, 4-3, 16-10, and 9-16, and their implications for fitting images. He highlights the challenges of fitting images with different accept ratios and presents two main options: cropping the image or adding empty spaces to fit the desired ratio.

Understanding Image Sizing and Positioning in CSS
Zakeer Hussain Syed provides a detailed explanation of the object fit and background properties in CSS for image sizing and positioning. He covers the concepts of cover and contain options, as well as the background size and position properties, highlighting their significance in developing media-heavy websites. The discussion also includes the drawbacks of the cover option and the use of margin auto for centering images without using display flex or background properties.

Understanding Margins and Centering Images
Zakeer Hussain Syed provides a detailed explanation of how margins apply to block level and inline level elements, particularly focusing on centering images. He explores the limitations of using margin auto and seeks input from Syed Farook and others for alternative solutions to center images vertically within their parent containers.

Understanding Position Absolute in CSS
Sohel Baig and Zakeer Hussain Syed discuss using a position substitute, and Zakeer explains the importance of moving an image to the top and understanding the technique. They also discuss the behavior of percentage values and the necessity of the parent having a position property when using position absolute. Syed Farook also contributes to the discussion, highlighting the importance of the parent having a position property for position absolute elements to fit properly.
* Image Positioning

Centering Elements Using CSS Properties
Zakeer Hussain Syed provides a detailed explanation of how to center elements using CSS properties, emphasizing the use of percentages and the transform property to achieve the desired result. He highlights the mathematical principles involved in the process and encourages understanding the concept thoroughly. Sohel Baig briefly mentions the inclusion of "after" and "before" in the discussion, to which Zakeer acknowledges and plans to cover in the next session.
* Centering Elements


Action Items:

* Zakeer Hussain Syed needs to disable form validation from the client side in the HTML.
* Zakeer Hussain Syed will cover HTML validation in the next session
* Zakeer Hussain Syed will cover responsive design in the next session
* Zakeer Hussain Syed will need to send something back.
* Zakeer Hussain Syed will cover Z-index and After/Before in the next session


## Key Questions:

**1. How does responsive design work?**

Responsive design is a web development approach aimed at crafting websites that adapt smoothly to different screen sizes and devices. This ensures optimal viewing and interaction experiences across desktops, tablets, and mobile phones. 

**Key Components:**

* **Fluid Grids:** Instead of fixed pixel widths, responsive layouts use percentages or relative units (like `em`, `rem`) for widths. This allows elements to resize proportionally with the screen.
* **Flexible Images:** Images are also set to maximum widths (using `max-width: 100%;`) so they don't exceed their container and scale down gracefully.
* **Media Queries:** These are CSS rules that apply different styles based on specific conditions, like screen size or orientation. They let you tailor your layout and styles for different devices.

**How it Works:**

1. **Browser Resizes:** When a user views your website, the browser detects the screen's width and height.
2. **Media Queries Trigger:** If the screen matches the conditions in your media queries, the browser applies the corresponding CSS styles.
3. **Content Adapts:** Elements resize, layouts change, and potentially even content is modified to fit the screen perfectly.

**Example:**

```css
/* Desktop styles */
.container {
  width: 960px;
}

/* Tablet styles (when screen width is 768px or less) */
@media (max-width: 768px) {
  .container {
    width: 720px;
  }
}

/* Mobile styles (when screen width is 480px or less) */
@media (max-width: 480px) {
  .container {
    width: 100%;
  }
}
```

**2. What is the reason to add rows in a text area?**

The `rows` attribute in a `<textarea>` element defines the visible height of the text area, i.e., how many lines of text are initially displayed. It's helpful for:

* **Visual Clarity:**  Providing enough visible space for users to easily enter the expected amount of text.
* **Usability:** Preventing users from having to scroll immediately within a small text area.
* **Design Consistency:** Maintaining a consistent visual appearance for forms and input areas.

**Example:**

```html
<textarea rows="5">
Enter your message here...
</textarea>
```

**3. How do you perfectly align an element center to the parent or screen?**

There are a few techniques to achieve perfect center alignment:

**Horizontal Centering:**

* **Flexbox:**

```css
.parent {
  display: flex;
  justify-content: center; /* Horizontally centers child elements */
}

.child {
  /* Additional styles for the child element */
}
```

* **Grid:**

```css
.parent {
  display: grid;
  place-items: center; /* Centers both horizontally and vertically */
}
```

* **Text Alignment (for inline elements):**

```css
.parent {
  text-align: center;
}
```

**Vertical Centering:**

* **Flexbox:**

```css
.parent {
  display: flex;
  align-items: center; /* Vertically centers child elements */
}
```

* **Grid:** (same as horizontal centering)

* **Absolute Positioning + Transforms:**

```css
.child {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
```

