---
date: '2024-12-23T15:03:47+08:00'
draft: false
title: 'Cambly Topics'
---

<div class="progress-bar-container" style="width: 100%; background-color: #f0f0f0; border-radius: 5px; margin: 20px 0;">
    <div id="progress-bar" class="progress-bar" style="width: 0%; height: 20px; background-color: #4CAF50; border-radius: 5px; text-align: center; color: white;">
        0%
    </div>
</div>

<div id="completion-status"></div>

# Topics:

- [x] Food & Dining
- [ ] Hobbies & Leisure Time
- [ ] Travel & Adventure
- [ ] Work & Career
- [ ] Family & Relationships
- [ ] Education & Learning
- [ ] Technology & Innovation
- [ ] Culture & Traditions
- [ ] Health & Wellness
- [ ] Environment & Sustainability

<script>
document.addEventListener('DOMContentLoaded', function() {
    function updateProgress() {
        const totalTasks = document.querySelectorAll('li').length;
        const completedTasks = document.querySelectorAll('li:has(input:checked)').length;
        const percentage = (completedTasks / totalTasks) * 100;
        
        const progressBar = document.getElementById('progress-bar');
        const completionStatus = document.getElementById('completion-status');
        
        progressBar.style.width = percentage + '%';
        progressBar.textContent = Math.round(percentage) + '%';
        completionStatus.textContent = `Progress: ${completedTasks}/${totalTasks}`;
    }

    // Initialize progress
    updateProgress();

    // Listen for checkbox changes
    document.addEventListener('change', function(e) {
        if (e.target.type === 'checkbox') {
            updateProgress();
        }
    });
});
</script>
