<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Football Streams - Live Matches</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            padding: 20px;
        }

        .container {
            max-width: 1400px;
            margin: 0 auto;
        }

        /* Header */
        .header {
            text-align: center;
            color: white;
            margin-bottom: 40px;
        }

        .header h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.2);
        }

        .header p {
            font-size: 1.1rem;
            opacity: 0.9;
        }

        /* Search Bar */
        .search-container {
            max-width: 600px;
            margin: 0 auto 30px;
            padding: 0 20px;
        }

        .search-box {
            display: flex;
            gap: 10px;
            background: white;
            border-radius: 50px;
            padding: 5px 20px;
            box-shadow: 0 5px 20px rgba(0,0,0,0.2);
        }

        .search-icon {
            align-self: center;
            color: #667eea;
            font-size: 1.2rem;
        }

        #searchInput {
            flex: 1;
            padding: 15px 10px;
            border: none;
            outline: none;
            font-size: 1rem;
            background: transparent;
        }

        .clear-search {
            background: none;
            border: none;
            color: #999;
            cursor: pointer;
            font-size: 1.2rem;
            padding: 0 10px;
            display: none;
        }

        .clear-search:hover {
            color: #667eea;
        }

        .search-stats {
            text-align: center;
            color: white;
            margin-top: 10px;
            font-size: 0.9rem;
            opacity: 0.9;
        }

        /* Loading Spinner */
        .loading {
            text-align: center;
            padding: 50px;
            color: white;
        }

        .spinner {
            border: 4px solid rgba(255,255,255,0.3);
            border-top: 4px solid white;
            border-radius: 50%;
            width: 50px;
            height: 50px;
            animation: spin 1s linear infinite;
            margin: 0 auto 20px;
        }

        @keyframes spin {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }

        /* Error Message */
        .error {
            background: rgba(255,0,0,0.1);
            border: 2px solid #ff4444;
            color: white;
            padding: 20px;
            border-radius: 10px;
            text-align: center;
            margin: 20px;
        }

        /* Match Grid */
        .matches-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(350px, 1fr));
            gap: 25px;
            margin-bottom: 30px;
        }

        /* Match Card */
        .match-card {
            background: white;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .match-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 40px rgba(0,0,0,0.3);
        }

        .match-header {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 20px;
        }

        .match-title {
            font-size: 1.3rem;
            font-weight: bold;
            margin-bottom: 10px;
            word-break: break-word;
        }

        .match-info {
            display: flex;
            justify-content: space-between;
            font-size: 0.85rem;
            opacity: 0.9;
        }

        .sources-list {
            padding: 15px;
            border-bottom: 1px solid #eee;
        }

        .source-btn {
            width: 100%;
            padding: 12px;
            margin: 5px 0;
            background: #f0f0f0;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            font-size: 1rem;
            transition: all 0.3s ease;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .source-btn:hover {
            background: #667eea;
            color: white;
            transform: translateX(5px);
        }

        .source-name {
            font-weight: bold;
        }

        .source-badge {
            background: #764ba2;
            color: white;
            padding: 3px 8px;
            border-radius: 12px;
            font-size: 0.75rem;
        }

        .streams-section {
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.3s ease;
        }

        .streams-section.active {
            max-height: 500px;
            overflow-y: auto;
        }

        .stream-item {
            padding: 12px 15px;
            border-top: 1px solid #eee;
            transition: background 0.2s ease;
        }

        .stream-info {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 8px;
        }

        .stream-language {
            font-weight: bold;
            color: #667eea;
        }

        .stream-quality {
            padding: 2px 8px;
            border-radius: 12px;
            font-size: 0.75rem;
            font-weight: bold;
        }

        .quality-hd {
            background: #4caf50;
            color: white;
        }

        .quality-sd {
            background: #ff9800;
            color: white;
        }

        .stream-url {
            font-size: 0.75rem;
            color: #666;
            word-break: break-all;
            font-family: monospace;
            margin-bottom: 8px;
        }

        .watch-btn {
            display: inline-block;
            padding: 8px 16px;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 0.85rem;
            transition: transform 0.2s, box-shadow 0.2s;
        }

        .watch-btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }

        /* Toast Notification */
        .toast {
            position: fixed;
            bottom: 30px;
            right: 30px;
            background: #4caf50;
            color: white;
            padding: 15px 25px;
            border-radius: 10px;
            box-shadow: 0 5px 20px rgba(0,0,0,0.2);
            transform: translateX(400px);
            transition: transform 0.3s ease;
            z-index: 1000;
            font-weight: bold;
        }

        .toast.show {
            transform: translateX(0);
        }

        /* No Results */
        .no-results {
            text-align: center;
            padding: 50px;
            color: white;
            background: rgba(255,255,255,0.1);
            border-radius: 15px;
            margin: 20px;
        }

        .no-results h3 {
            font-size: 1.5rem;
            margin-bottom: 10px;
        }

        /* Stats */
        .stats {
            text-align: center;
            color: white;
            margin-top: 30px;
            padding: 20px;
            background: rgba(0,0,0,0.2);
            border-radius: 10px;
        }

        @media (max-width: 768px) {
            .matches-grid {
                grid-template-columns: 1fr;
            }
            
            .header h1 {
                font-size: 1.8rem;
            }
            
            .search-box {
                padding: 5px 15px;
            }
            
            .toast {
                bottom: 20px;
                right: 20px;
                left: 20px;
                text-align: center;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>⚽ Live Football Streams</h1>
            <p>Find and watch live matches from around the world</p>
        </div>

        <div class="search-container">
            <div class="search-box">
                <span class="search-icon">🔍</span>
                <input type="text" id="searchInput" placeholder="Search for your favorite team or match..." autocomplete="off">
                <button class="clear-search" id="clearSearch">✕</button>
            </div>
            <div class="search-stats" id="searchStats"></div>
        </div>

        <div id="content">
            <div class="loading">
                <div class="spinner"></div>
                <p>Loading matches...</p>
            </div>
        </div>
    </div>

    <!-- Toast Notification -->
    <div id="toast" class="toast">
        🔗 Link copied to clipboard!
    </div>

    <script>
        let allMatches = [];
        let filteredMatches = [];

        async function fetchMatches() {
            try {
                const response = await fetch('https://streamed.pk/api/matches/football');
                if (!response.ok) throw new Error('Failed to fetch matches');
                const matches = await response.json();
                
                if (matches.length === 0) {
                    throw new Error('No matches found');
                }
                
                allMatches = matches;
                filteredMatches = [...allMatches];
                renderMatches(filteredMatches);
                setupSearch();
            } catch (error) {
                showError(error.message);
            }
        }

        function setupSearch() {
            const searchInput = document.getElementById('searchInput');
            const clearButton = document.getElementById('clearSearch');
            
            searchInput.addEventListener('input', (e) => {
                const searchTerm = e.target.value.toLowerCase().trim();
                
                if (searchTerm === '') {
                    clearButton.style.display = 'none';
                    filteredMatches = [...allMatches];
                } else {
                    clearButton.style.display = 'block';
                    filteredMatches = allMatches.filter(match => 
                        match.title.toLowerCase().includes(searchTerm)
                    );
                }
                
                renderMatches(filteredMatches);
                updateSearchStats(searchTerm, filteredMatches.length);
            });
            
            clearButton.addEventListener('click', () => {
                searchInput.value = '';
                clearButton.style.display = 'none';
                filteredMatches = [...allMatches];
                renderMatches(filteredMatches);
                updateSearchStats('', filteredMatches.length);
                searchInput.focus();
            });
        }
        
        function updateSearchStats(searchTerm, resultCount) {
            const statsDiv = document.getElementById('searchStats');
            if (searchTerm) {
                statsDiv.textContent = `Found ${resultCount} match${resultCount !== 1 ? 'es' : ''} for "${searchTerm}"`;
            } else {
                statsDiv.textContent = `${resultCount} match${resultCount !== 1 ? 'es' : ''} available`;
            }
        }

        function renderMatches(matches) {
            const contentDiv = document.getElementById('content');
            
            if (!matches || matches.length === 0) {
                contentDiv.innerHTML = `
                    <div class="no-results">
                        <h3>😕 No matches found</h3>
                        <p>Try searching for a different team or match</p>
                    </div>
                `;
                return;
            }

            let totalStreams = 0;
            matches.forEach(match => {
                if (match.sources) totalStreams += match.sources.length;
            });

            const html = `
                <div class="matches-grid">
                    ${matches.map((match, index) => renderMatchCard(match, index)).join('')}
                </div>
                <div class="stats">
                    📊 ${matches.length} Matches | 🎥 ${totalStreams} Sources Available
                </div>
            `;
            
            contentDiv.innerHTML = html;
        }

        function renderMatchCard(match, index) {
            if (!match.sources || match.sources.length === 0) {
                return `
                    <div class="match-card">
                        <div class="match-header">
                            <div class="match-title">${escapeHtml(match.title)}</div>
                            <div class="match-info">
                                <span>⚠️ No streams available</span>
                            </div>
                        </div>
                    </div>
                `;
            }

            return `
                <div class="match-card" data-match-id="${index}">
                    <div class="match-header">
                        <div class="match-title">${escapeHtml(match.title)}</div>
                        <div class="match-info">
                            <span>🎥 ${match.sources.length} source(s)</span>
                        </div>
                    </div>
                    <div class="sources-list">
                        ${match.sources.map((source, sourceIndex) => `
                            <button class="source-btn" onclick="toggleStreams(${getOriginalMatchIndex(match)}, ${sourceIndex})">
                                <span class="source-name">${escapeHtml(source.source)}</span>
                                <span class="source-badge">${source.id}</span>
                            </button>
                            <div id="streams-${getOriginalMatchIndex(match)}-${sourceIndex}" class="streams-section">
                                <div class="loading-streams" style="padding: 10px; text-align: center; color: #999;">
                                    Loading streams...
                                </div>
                            </div>
                        `).join('')}
                    </div>
                </div>
            `;
        }
        
        function getOriginalMatchIndex(match) {
            return allMatches.findIndex(m => m.title === match.title);
        }

        async function toggleStreams(matchIndex, sourceIndex) {
            const streamsDiv = document.getElementById(`streams-${matchIndex}-${sourceIndex}`);
            
            if (streamsDiv.classList.contains('active')) {
                streamsDiv.classList.remove('active');
                return;
            }

            streamsDiv.classList.add('active');
            
            const match = allMatches[matchIndex];
            const source = match.sources[sourceIndex];
            
            try {
                const response = await fetch(`https://streamed.pk/api/stream/${source.source}/${source.id}`);
                const streams = await response.json();
                
                if (streams.length === 0) {
                    streamsDiv.innerHTML = '<div style="padding: 10px; text-align: center; color: #999;">No streams available</div>';
                    return;
                }
                
                streamsDiv.innerHTML = streams.map(stream => `
                    <div class="stream-item">
                        <div class="stream-info">
                            <span class="stream-language">🌐 ${escapeHtml(stream.language || 'Unknown')}</span>
                            <span class="stream-quality ${stream.hd ? 'quality-hd' : 'quality-sd'}">
                                ${stream.hd ? 'HD' : 'SD'}
                            </span>
                        </div>
                        <div class="stream-url">
                            ${stream.streamNo ? `Stream #${stream.streamNo} - ` : ''}${escapeHtml(stream.embedUrl)}
                        </div>
                        <button class="watch-btn" onclick="copyToClipboard('${escapeHtml(stream.embedUrl)}', '${escapeHtml(match.title)} - ${stream.language}')">
                            📋 Copy Stream Link
                        </button>
                    </div>
                `).join('');
                
            } catch (error) {
                streamsDiv.innerHTML = `<div style="padding: 10px; text-align: center; color: #f44336;">Error loading streams: ${error.message}</div>`;
            }
        }

        async function copyToClipboard(url, title) {
            try {
                await navigator.clipboard.writeText(url);
                showToast(`✅ Copied: ${title}`);
                
                // Optional: Also log to console for debugging
                console.log(`Copied stream link for ${title}: ${url}`);
            } catch (err) {
                // Fallback for older browsers
                const textarea = document.createElement('textarea');
                textarea.value = url;
                document.body.appendChild(textarea);
                textarea.select();
                document.execCommand('copy');
                document.body.removeChild(textarea);
                showToast(`✅ Copied: ${title}`);
            }
        }

        function showToast(message) {
            const toast = document.getElementById('toast');
            toast.textContent = message;
            toast.classList.add('show');
            
            setTimeout(() => {
                toast.classList.remove('show');
            }, 3000);
        }

        function showError(message) {
            const contentDiv = document.getElementById('content');
            contentDiv.innerHTML = `
                <div class="error">
                    <strong>⚠️ Error:</strong> ${escapeHtml(message)}<br>
                    <button onclick="location.reload()" style="margin-top: 10px; padding: 8px 16px; background: white; border: none; border-radius: 5px; cursor: pointer;">Retry</button>
                </div>
            `;
        }

        function escapeHtml(str) {
            if (!str) return '';
            return str.replace(/[&<>]/g, function(m) {
                if (m === '&') return '&amp;';
                if (m === '<') return '&lt;';
                if (m === '>') return '&gt;';
                return m;
            }).replace(/[\uD800-\uDBFF][\uDC00-\uDFFF]/g, function(c) {
                return c;
            });
        }

        // Initialize
        fetchMatches();
    </script>
</body>
</html>