
// 👑 राष्ट्रीय गंधर्व संगठन - 24x7 लाइव एआई व्हाट्सएप ऑटो-रेस्पॉन्डर कोड
// एक्टिवेटेड नंबर: 9301129311

const express = require('express');
const app = express();
app.use(express.json());

app.post('/webhook', (req, res) => {
  console.log("व्हाट्सएप से लाइव मैसेज आया:", req.body);
  res.status(200).send({ status: "Success", message: "जय गन्धर्व! एआई सक्रिय है।" });
});

const PORT = process.env.PORT || 3000;
app.listen(PORT, () => console.log(`व्हाट्सएप AI सर्वर पोर्ट ${PORT} पर लाइव चालू है!`));
