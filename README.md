<!DOCTYPE html>                    
</div>                    
<h3 class="feature-title">更新日志</h3>                    
<p class="feature-desc">2025.6.4 修复高版本无法使用鞘翅，右键地面回弹问题</p >                    
<p class="feature-desc">2025.6.8 建立C3K6官方网站</p >                
</div>
        </section>        
<footer>            
<p>© 于2025年正式开服 | 1.20.1核心版本</p >            
<p>挑战性 · 战斗 · 友善</p >        
</footer>    
<script>        
// 交互按钮功能        
const actionBtn = document.getElementById('actionBtn');                
actionBtn.addEventListener('click', function() {            
// 平滑滚动到下一个部分            
window.scrollTo({            
top: document.body.scrollHeight,                
behavior: 'smooth'            
});                        
// 保留原有的粒子效果（可选）        
});                
// 粒子效果函数（保留原有功能）        
function createParticles() {            
const colors = ['#2c7744', '#1e5799', '#207cca', '#2989d8', '#5ac8aa'];                        
for (let i = 0; i < 50; i++) {                
const particle = document.createElement('div');                
particle.style.position = 'fixed';                
particle.style.width = '10px';                
particle.style.height = '10px';                
particle.style.backgroundColor = colors[Math.floor(Math.random() * colors.length)];                
particle.style.borderRadius = '50%';                
particle.style.left = `${Math.random() * 100}vw`;                
particle.style.top = `${Math.random() * 100}vh`;                
particle.style.pointerEvents = 'none';                
particle.style.zIndex = '999';                
particle.style.boxShadow = '0 0 15px currentColor';                                
document.body.appendChild(particle);                                
const animation = particle.animate([                    
{ transform: 'scale(0)', opacity: 1 },                    
{ transform: 'scale(1.5)', opacity: 0.7 },                    
{ transform: 'scale(3)', opacity: 0 }                
], {                    
duration: 1500,                    
easing: 'ease-out'                
});                                
animation.onfinish = () => particle.remove();            
}        
}    
</script>
</body>
</html>
