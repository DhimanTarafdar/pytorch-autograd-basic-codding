# PyTorch Autograd Notebook

এই নোটবুকে আমি PyTorch এর Autograd বিষয়টা প্র্যাকটিস করেছি। এখানে মূলত দেখানো হয়েছে কিভাবে tensor তৈরি করতে হয়, কিভাবে `requires_grad=True` দিলে PyTorch gradient ট্র্যাক করে, এবং `backward()` কল করলে কিভাবে gradient হিসাব করে।

আমি কিছু সিম্পল উদাহরণ করেছি যেমন:
- একটি tensor নিয়ে তার উপর গাণিতিক অপারেশন করা
- loss calculate করা
- backward() ব্যবহার করে gradient বের করা
- একই ভেরিয়েবলের উপর একাধিকবার backward() কল করলে কি হয় তা দেখা
- কেন কিছু ক্ষেত্রে backward() কাজ করে না সেটাও বোঝার চেষ্টা করেছি

এই নোটবুকটি মূলত আমার নিজের শেখার জন্য বানানো। এখানে step by step ভাবে PyTorch কিভাবে gradient calculate করে সেটা বোঝার চেষ্টা করেছি।
```
