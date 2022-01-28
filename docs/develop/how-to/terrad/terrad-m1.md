# Install `terrad` for M1 mac

1. Navigate to [https://github.com/terra-money/core/tags](https://github.com/terra-money/core/tags) and click on the latest release. 
2. Download the correct .tar.gz file for your computer's OS.
3. Open terminal and navigate to the downloaded file: 
    
    `cd Downloads/terra_0.5.1_Darwin_x86_64/`
    
4. Add `.dylib` to /lib.
    
    Intel based macs:  `cp libwasmvm.dylib /usr/local/lib`
    
    M1 macs:  
    
    `cd /usr/local`
    
    `mkdir lib`
    
    `cp libwasmvm.dylib /usr/local/lib`
    
    Note: if you receive a `permission denied` message, add `sudo` before each command. 
    
5. Run `./terrad`
    
    If a security warning occurs:
    
   1. Navigate to system preferences→security & privacy. 
   2. Under the "General" tab, click "Allow anyway." 
   3. Run `./terrad` again. 
   4. When prompted, click "open." Repeat for other security errors. 
6. Add `terrad` to your path:
    
   - Intel based macs: `cp terrad /usr/local/bin`
    
   - M1 macs: 
    
   `cd /usr/local`
    
   `mkdir bin`
    
   `cp terrad /usr/local/bin`
    
   :::{Note}
   If you receive a `permission denied` message, add `sudo` before each command. 
   :::

7. Run `terrad`