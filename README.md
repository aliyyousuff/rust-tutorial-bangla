# rust-tutorial-bangla

রাষ্ট নতুন একটি প্রোগ্রামিং ল্যাংগুয়েজ, যার জনপ্রিয়তা প্রতিনিয়ত বাড়ছে।  বাংলাতে রাষ্ট নিয়ে কোনো টিউটোরিয়াল নেই।  সে জন্য এই প্রজেক্ট এর উদ্ভব।  আসলে বাংলাতে একদম নতুন--যারা কখনো প্রোগ্রামিং করেননি--তাদের জন্য ভালো কোনো টিউটোরিয়াল নেই, তাই এই টিউটোরিয়াল সিরিজের মাধ্যমে প্রোগ্রামিং কে আনন্দ দায়ক এবং একদম সহজ করে তোলার চেষ্টা করা হয়েছে।  যাতে ক্লাস ফাইভ এর একজন ছাত্রও যেন প্রোগ্রামিং বুঝতে পারে।  

আপনি যদি এই প্রজেক্টে অবদান/কান্ট্রিবিউট করতে চান তাহলে নিচের স্টেপ গুলো ফলো করে আপনি আপনার কম্পিউটারে এনভায়রনমেন্ট সেটআপ করে নিতে পারেন।  তার আগে অবশ্য এই প্রজেক্টটি ক্লোন করে আপনার কম্পিউটারে নিতে হবে। 

এই টিউটোরিয়ালের বাংলা টাইপ করা হয়েছে ফোনেটিক ব্যবহার করে, বেশিরভাগ টাইপ করা হয়েছে এই [লিংক](https://www.google.com/intl/bn/inputtools/try/) থেকে। 

সব গুলো টিউটোরিয়াল মার্কডাউন ফাইল ফরম্যাটে সেভ করা হয়েছে।  আর মার্কডাউন রেন্ডার/রিড করা হয়েছে VS Studio Code দিয়ে।  VS Studio Code এর একটি এক্সটেনশন যার নাম হচ্ছে `Markdown Preview Enhanced` ইনস্টল করা হয়েছে।  এই এক্সটেনশন দিয়ে  মার্কডাউন ফাইলের বাংলা লিখা রিড করতে গেলে বাংলা ফন্ট ভেঙে যায়, সেটার সমাধান নিছে দেওয়া হল:

- আপনার কম্পিউটারে `kalpurush` ফন্ট ডাউনলোড করতে হবে, ডাউনলোড [লিংক](https://www.omicronlab.com/bangla-fonts.html)
- VS Studio Code ওপেন করে `ctrl` + `Shift` + `P`  চেপে ধরলে `Markdown Preview Enhanced: Customized CSS ` সিলেক্ট করে ক্লিক করুন।
- তারপর দেখবেন VS Studio Code এ style.less নামের একটি ফাইল ওপেন হবে, সেখানে নিচের কোড গুলো কপি পেস্ট করুন:

```

/* Please visit the URL below for more information: */
/*   https://shd101wyy.github.io/markdown-preview-enhanced/#/customize-css */

@font-face {
  font-family: kalpurush;
  src: url("/home/yousuf/Downloads/kalpurush.ttf");
}
  .markdown-preview.markdown-preview {
    font-family: kalpurush, sans-serif;
  
    h1,
    h2,
    h3,
    h4,
    h5,
    h6,
    pre,
    code {
      font-family: kalpurush, sans-serif;
    }
  }
```

- আপনাকে শুধু এই `src: url("/home/yousuf/Downloads/kalpurush.ttf");` লাইনে একটু পরিবর্তন আনতে হবে, আপনার কম্পিউটারে যেখানে ফন্ট টি ডাউনলোড করেছেন সেখানের path টি এখানে বসিয়ে দিন।  এখানে আমার উবুন্টু কম্পিউটারের ডাউনলোড ফোল্ডারের path টি বসানো।  

- আপনাকে রাস্ট কম্পাইলার ইন্সটল করে নিতে হবে, সেটার [লিংক](https://www.rust-lang.org/tools/install) । 

# ভবিষ্যৎ পরিকল্পনা
মোটামুটি কয়েক অধ্যায় লিখা হয়ে গেলে আমাদের একটি ওয়েবসাইট খোলার পরিকল্পনা আছে, সেখানে আমরা সব টিউটোরিয়াল বাংলাভাষী সব মানুষের জন্য উন্মুক্ত করে দিব। 