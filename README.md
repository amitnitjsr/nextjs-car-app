# Build and Deploy a Modern Next.js 13 Application | React, Next JS 13, TypeScript, Tailwind CSS
![Car Showcase](https://i.ibb.co/GxvFJDZ/Thumbnail.png)

## Introduction
The demand for Next.js 13 applications peaked! Now is the perfect time to build a state-of-the-art modern application that leverages all of the latest and greatest of what Next 13 has to offer, leveraging features such as server-side rendering and the app router. 
 
Alongside building this application, you'll also learn how to:
- Use Next.js 13 App Router and Server Side Rendering
- Implement Advanced Search Functionality
- Create Filtering Capabilities
- Optimize Metadata and SEO
- Create custom filter, combobox, and modal elements
- Maintain a well-organized file and folder structure.
- Embrace the principles of writing clean code.

## Want to land your dream programming job in 3 - 6 months?
⭐ JSM Masterclass Experience - https://jsmastery.pro/masterclass
Become a Software Engineer. Guaranteed.

const axios = require('axios');

const options = {
  method: 'GET',
  url: 'https://cars-by-api-ninjas.p.rapidapi.com/v1/cars',
  params: {model: 'corolla'},
  headers: {
    'X-RapidAPI-Key': '7e15dcea92msh21d705098d10b51p11238djsn669d46e3e6d4',
    'X-RapidAPI-Host': 'cars-by-api-ninjas.p.rapidapi.com'
  }
};

try {
	const response = await axios.request(options);
	console.log(response.data);
} catch (error) {
	console.error(error);
}
