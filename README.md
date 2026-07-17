# Prompt Library v1: Customer Support Automation

Welcome to the **Prompt Library v1**. This repository contains a reusable, production-grade prompt template engineered using the **Role + Context + Task + Format + Constraints** framework. It is designed to help customer support teams generate consistent, empathetic, and policy-aligned email responses efficiently by simply swapping dynamic variables.

---

## 1. The Core Master Template

This is the foundational framework. The placeholders wrapped in `{{variable_name}}` represent the inputs that change based on each individual support ticket.

```text
[ROLE]
You are an expert Customer Support Specialist for {{Company_Name}}, known for being {{Tone}} and highly efficient.

[CONTEXT]
A customer has reached out with the following issue: "{{Customer_Issue}}". 
The customer's current mood/sentiment is {{Customer_Mood}}.
Our internal company policy for this situation is: "{{Company_Policy}}".

[TASK]
Draft a complete response to the customer that addresses their issue completely, acknowledges their feelings, and provides the next steps based on our policy.

[FORMAT]
- Email format (Subject Line + Body + Sign-off)
- Use clear paragraph breaks
- Use bullet points if listing steps

[CONSTRAINTS]
- Do not make up facts or promises outside of the stated policy.
- Keep the response under {{Word_Count}} words.
- Use placeholders like [Customer Name] or [Agent Name] where specific names are needed.
2. Tested Prompts & AI Outputs (5 Test Cases)
Case 1: Delayed Shipping (Angry Customer)
Variables:

{{Company_Name}}: SwiftCart Electronics

{{Tone}}: Empathetic and reassuring

{{Customer_Issue}}: Order #1042 is 5 days late; tracking hasn't updated.

{{Customer_Mood}}: Extremely frustrated and angry

{{Company_Policy}}: Apologize, offer a $10 refund on shipping, check internal tracker.

{{Word_Count}}: 150 words

AI Generated Output:
Subject: Update regarding your SwiftCart Order #1042

Dear Ali Khan,

I completely understand your frustration regarding the delay of your Order #1042. It is incredibly disappointing when tracking doesn't update, and I sincerely apologize for the stress this has caused.

To help make this right, I have processed a $10 refund on your shipping fees. I have also personally checked our internal manual tracker, which shows your package is currently at our main regional hub and is scheduled for delivery within the next 48 hours.

Thank you for your patience as we get this sorted out for you.

Best regards,

Danish Hanif

SwiftCart Support Team

Case 2: Wrong Item Received (Disappointed Customer)
Variables:

{{Company_Name}}: Threads Clothing Co.

{{Tone}}: Apologetic and action-oriented

{{Customer_Issue}}: Ordered a medium blue jacket, received a small red sweater.

{{Customer_Mood}}: Disappointed but polite

{{Company_Policy}}: Send a prepaid return label, ship the correct jacket immediately at no extra cost.

{{Word_Count}}: 150 words

AI Generated Output:
Subject: Resolving your recent Threads Clothing Co. order

Hi Aisha Fatima,

Thank you for reaching out and letting us know. I am so sorry for the mix-up with your order! I know how disappointing it is to receive the wrong item.

We want to fix this for you right away. Here is what we are doing:

Your Correct Jacket: I have rushed the shipment for your medium blue jacket. It is on its way at no extra charge.

The Return: Attached to this email, you will find a prepaid return label. Please use it to send the red sweater back to us whenever you can.

Thank you for being so understanding!

Warmly,

Danish Hanif

Threads Clothing Co.

Case 3: Feature Request (Hopeful Tech User)
Variables:

{{Company_Name}}: TaskFlow SaaS

{{Tone}}: Enthusiastic, polite, and appreciative

{{Customer_Issue}}: Asking if TaskFlow can add a dark mode feature.

{{Customer_Mood}}: Excited, loves the app but wants this feature

{{Company_Policy}}: Thank them, explain it's in our Q4 roadmap, and add them to the beta notification list.

{{Word_Count}}: 120 words

AI Generated Output:
Subject: Great news about Dark Mode in TaskFlow!

Hi Bilal Raza,

Thank you so much for reaching out! We are thrilled to hear that you love using TaskFlow.

To answer your question: Yes, dark mode is officially on our Q4 roadmap! Our design team is currently working on it, and it looks amazing. I have gone ahead and added your email to our exclusive beta notification list so you can try it out before anyone else.

Thanks for helping us make TaskFlow better!

Cheers,

Danish Hanif

TaskFlow Team

Case 4: Subscription Cancellation (Neutral Customer)
Variables:

{{Company_Name}}: FitLife App

{{Tone}}: Respectful, brief, and helpful

{{Customer_Issue}}: Wants to cancel subscription because they don't have time to work out.

{{Customer_Mood}}: Neutral/indifferent

{{Company_Policy}}: Process cancellation immediately, confirm no further charges, mention they can reactivate anytime.

{{Word_Count}}: 100 words

AI Generated Output:
Subject: Confirmation of your FitLife subscription cancellation

Hello Maryam Shah,

As requested, I have processed the cancellation of your FitLife subscription today.

You will still have full premium access to the app until the end of your current billing cycle, after which no further charges will be made. Please note that your workout history will be saved safely, so you can reactivate your account anytime you feel ready to jump back in.

We wish you all the best on your fitness journey!

Best,

Danish Hanif

FitLife Support

Case 5: Out of Stock Inquiry (Eager Customer)
Variables:

{{Company_Name}}: GlowSkincare

{{Tone}}: Informative, warm, and helpful

{{Customer_Issue}}: Vitamin C Serum is out of stock; wants to know when it's coming back.

{{Customer_Mood}}: Curious and eager to buy

{{Company_Policy}}: Inform them restock is in 2 weeks, offer a 10% discount code for the wait, give link to "notify me" page.

{{Word_Count}}: 130 words

AI Generated Output:
Subject: Vitamin C Serum Restock Update!

Hi Sana Imran,

Thank you for your interest in our Vitamin C Serum! It's one of our favorites too, so I completely understand why you're eager to get your hands on it.

Our team is working hard, and the serum will be fully restocked in exactly two weeks. To thank you for your patience, please use the code GLOW10 at checkout for 10% off your next purchase.

You can also click [here] to sign up for instant email alerts the second it lands back on our shelves.

Have a glowing day!

Warmly,

Danish Hanif

GlowSkincare Team

3. Demo Video
Since this project requires a live walkthrough, a short, silent screen-recording demo showing the repository layout and demonstrating how variables function within the template has been recorded.

👉 [Click Here to Watch the Demo Video](https://www.linkedin.com/posts/danish-hanif-5839583bb_promptengineering-aiautomation-neurofivesolutions-ugcPost-7483943615459684353-UBc5/?utm_source=share&utm_medium=member_desktop&rcm=ACoAAGZ6ajMBNDJWRNIInsosvdqlP4Mh3ICMuDU)
