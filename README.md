# 🌩️ Cloudku Uploader

Cloudku Uploader is a lightweight Node.js package that makes it easy to upload files to [CloudkuImages](https://cloudkuimages.com).  
It supports both **CommonJS (CJS)** and **ECMAScript Modules (ESM)**.

[![npm version](https://img.shields.io/npm/v/cloudku-uploader.svg)](https://www.npmjs.com/package/cloudku-uploader)  
[![License: MIT](https://img.shields.io/badge/License-Custom%20MIT-blue.svg)](LICENSE)  
[![Node.js](https://img.shields.io/badge/Node.js-16%2B-brightgreen)](https://nodejs.org/)  
[![Support CJS & ESM](https://img.shields.io/badge/Supports-CJS%20%7C%20ESM-orange)](#)

---

## 📦 Installation
```bash
npm install cloudku-uploader
```

---

## 🚀 Usages

### **1. CommonJS (CJS)**

```js
const uploadFile = require('cloudku-uploader');
const fs = require('fs');

(async () => {
  const buffer = fs.readFileSync('example.jpg');
  const result = await uploadFile(buffer, 'example.jpg');
  console.log(result);
})();
```

### **2. ECMAScript Modules (ESM)**

```js
import uploadFile from 'cloudku-uploader';
import fs from 'fs';

(async () => {
  const buffer = fs.readFileSync('example.jpg');
  const result = await uploadFile(buffer, 'example.jpg');
  console.log(result);
})();
```

---

## 📌 Api Responses Structure

|   Field    | Type   |            Description                 |
| ---------- | ------ | -------------------------------------  |
| `status`   | String | Upload status: ("success") / ("Error)  |
| `url`      | String | Direct link to uploaded file           |
| `fileName` | String | Final uploaded file name               |
| `size`     | Number | File size in readable format (KB, MB)  |
| `type`     | String | MIME type of the file                  |
| `info`     | String | Official channel for info & support    |

📥 API Response

```json
{
  "status": "success",
  "url": "https://cloudkuimages.com/uploads/example.jpg",
  "fileName": "example.jpg",
  "size": "1.27 MB",
  "type": "image/jpeg",
  "information": "https://cloudkuimages.com/ch"
}
```

---

## 🛡 License & Legal
This package is under a Custom MIT License:

You may not copy, modify, resell, or redistribute this package without explicit permission.
Violators will be prosecuted under Indonesian and international copyright law.

📄 See full LICENSE file for complete details.


---

## 🙋 Support & Contact
Got questions or feedback? Reach out:
🌐 Website: [Cloudkuimages](https://cloudkuimages.guru)
💬 WhatsApp: [channels](https://cloudkuimages.guru/ch)
🎲Github: [GitHub](https://github.com/AlfiCloud)

---

## 👨‍💻 Author

- **AlfiDev** - [GitHub](https://github.com/AlfiCloud) | [Website](https://cloudkuimages.guru)
