- 👋 Hi, I’m @Liar-we
- 👀 I’m interested in Art & Science.
- 🌱 I’m currently learning about myself (universe).
- 💞️ I want to collaborate on various content creation (audio/video) and online business projects.
- 📫 you can find me as Vedvert_ on Instagram.
- 😄 Pronouns: HE/HIM.
- ⚡ Fun fact: the water and air we consume are much older than the sun.
- 

<!---
Liar-we/Liar-we is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
function twoSum(nums, target) {
    const numMap = new Map();

    for (let i = 0; i < nums.length; i++) {
        const complement = target - nums[i];
        if (numMap.has(complement)) {
            return [numMap.get(complement), i];
        }
        numMap.set(nums[i], i);
    }

    // If no solution is found
    return null;
}
